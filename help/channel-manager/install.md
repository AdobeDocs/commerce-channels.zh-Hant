---
title: 安裝 [!DNL Channel Manager]
description: 安裝Channel Manager擴展。
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4509528d1b084c9a91fd6be0d0a863782edb3bdd
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# 安裝通道管理器

查看 [先決條件](onboard.md#prerequisites) 並在安裝Channel Manager之前收集所需資訊。

## 更新最小穩定性設定

安裝擴展之前，請更新 `minimum-stability` 您 `composer.json` 檔案，以便您可以使用Composer安裝早期版本的Channel Manager。

要更新配置，請將以下行添加到 `composer.json` 的子菜單。

```json
{
   "minimum-stability": "alpha",
   "prefer-stable": true
}
```

## 安裝擴展

Channel Manager的安裝說明取決於是在內部部署Adobe Commerce還是在雲基礎架構上部署Magento Open Source。

- 在 [本地實例](#install-on-an-on-premises-instance)。

- 在 [[!DNL Adobe Commerce] 在雲基礎架構實例上](#install-adobe-commerce-on-cloud-infrastructure)

這兩種方法都要求您使用命令行介面(CLI)。

>[!NOTE]
>
>有關安裝幫助 [!DNL Commerce] 使用CLI的軟體，請參見 [常規CLI安裝](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}。

### 在本地實例上安裝

請使用以下說明在Adobe Commerce和Magento Open Source平台上安裝。

1. 登錄到 [!DNL Commerce] 伺服器 [具有權限的用戶](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target=&quot;_blank&quot;}要寫入 [!DNL Commerce] 檔案系統。

1. 將您的網站放入 [維護模式](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target=&quot;_blank&quot;}。

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 從 [!DNL Commerce] 項目根目錄，將Channel Manager添加到 `composer.json`。

   ```bash
    $ composer require magento/channel-manager --no-update
   ```

1. 如果出現提示，請輸入您的 [!DNL Commerce] 帳戶。

   您的公鑰是您的用戶名；你的私鑰是你的密碼。

1. 更新依賴項並安裝擴展。

   ```bash
   $ composer update
   ```

   的 `composer update` 命令更新所有依賴關係。 要僅更新與Channel Manager相關的依賴項，請改用以下命令： `composer update magento/channel-manager`。

1. 等待Composer完成更新項目依賴項並解決所有錯誤。

1. 驗證安裝

   ```bash
   $ bin/magento module:status channel-manager
   ```

   示例響應：

   ```terminal
   Module is disabled
   ```

1. 註冊擴展。

   ```bash
   $ bin/magento setup:upgrade
   ```

1. 如果出現提示，請重新編譯 [!DNL Commerce] 項目。

   ```bash
   $ bin/magento setup:di:compile
   ```

1. 驗證是否已啟用擴展：

   ```bash
   $ bin/magento module:status channel-manager
   ```

   示例響應：

   ```bash
   Module is enabled
   ```

1. 清除快取。

   ```bash
   $ bin/magento cache:clean
   ```

1. 禁用維護模式。

   ```bash
    $ bin/magento maintenance:disable
   ```

### 在Adobe Commerce上安裝雲基礎架構實例

在向雲實例添加擴展時在開發分支中工作。

有關使用分支的幫助，請參見 [開始建立分支](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted)Adobe Commerce開發人員文檔中的{target=&quot;_blank&quot;}。

安裝期間，副檔名(`&lt;VendorName>\_&lt;ComponentName>`) [app/etc/config.php](https://devdocs-beta.magento.com/guides/v2.3/config-guide/config/config-php.html){target=&quot;_blank&quot;}檔案。 您不需要直接編輯檔案。

1. 在本地工作站上，更改為雲項目根目錄。

1. 建立或簽出開發 [分支](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;}。

1. 使用Composer名稱，將擴展添加到 `require` 的下界 `composer.json` 的子菜單。

   ```bash
   $ composer require magento/channel-manager --no-update
   ```

1. 添加、提交和推送代碼更改 — 包括對 `composer.lock` 和 `composer.json` 的子菜單。

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m “Install channel manager extension” 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. 構建和部署完成後，使用SSH登錄到遠程環境並驗證擴展安裝是否正確。

   ```bash
   $ bin/magento module:status channel-manager
   ```

   示例響應：

   ```terminal
   Module is enabled
   ```

1. 安裝成功後，登錄到 [!UICONTROL Admin] 至 [配置Commerce Services連接器](connect.md)。

   >[!NOTE]
   >
   >有關將Channel Manager更新為新版本的說明，請參見 [升級模組和擴展](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target=&quot;_blank&quot;}。


## 故障排除

使用以下資訊可解決在Channel Manager安裝過程中發生的錯誤。

### 合成器鍵不正確

如果 [訪問密鑰](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}用於向Composer儲存庫進行身份驗證無效，或未連結到 [!DNL MAGE ID] 以前是註冊的 [!DNL Channel Manager] 服務，顯示以下錯誤。

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

檢查密鑰配置：

1. 查找 `auth.json` 檔案：

   ```bash
   $ composer config –global home
   ```

1. 查看 `auth.json` 的子菜單。

   ```bash
   $ cat /path/to/auth.json
   ```

1. 驗證auth.json中的憑據是否匹配 [與MAGE ID關聯的鍵](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}用於註冊Channel Manager服務。

### 記憶體不足，無法用於PHP

如果系統沒有為PHP分配足夠的記憶體，則會顯示以下錯誤。

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

使用以下任一方法解決記憶體問題：

- [增加PHP的記憶體限制](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit)環境中的{target=&quot;_blank&quot;} `php.ini` 的子菜單。 另外，驗證Commerce實例是否具有 [推薦值](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html){target=&quot;_blank&quot;}，以獲取其他PHP設定。

- 從命令行指定記憶體限制。

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   例如：

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### 缺少視圖

如果您對丟失 `process_catalog_exporter_view` 在Channel Manager安裝過程中，嘗試 [刷新索引器](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target=&quot;_blank&quot;}。

```bash
php bin/magento indexer:refresh
```

### 雲部署錯誤

有關將擴展部署到雲的問題，請參見 [擴展部署失敗](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target=&quot;_blank&quot;}。
