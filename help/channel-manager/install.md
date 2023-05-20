---
title: '''安裝 [!DNL Channel Manager]"'
description: '''安裝[!DNL Channel Manager] 擴展。'
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 96016b086a2c6567fab66b497892022f172f4bdd
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# 安裝 [!DNL Channel Manager]

查看 [要求](onboard.md#requirements) 並在安裝Channel Manager之前收集所需資訊。

## 安裝擴展

Channel Manager的安裝說明取決於是在內部部署Adobe Commerce還是在雲基礎架構上部署Magento Open Source。

- 在 [本地實例](#install-on-an-on-premises-instance)。

- 在 [[!DNL Adobe Commerce] 在雲基礎架構實例上](#install-adobe-commerce-on-cloud-infrastructure)

這兩種方法都要求您使用命令行介面(CLI)。

>[!NOTE]
>
>有關安裝的幫助 [!DNL Commerce] 使用CLI的軟體，請參見 [常規CLI安裝](https://devdocs.magento.com/extensions/install/){target="_blank"}。

### 在本地實例上安裝

使用以下說明進行安裝 [!DNL Channel Manager] Adobe Commerce和Magento Open Source到一個內部案件。

1. 登錄到 [!DNL Commerce] 伺服器 [具有權限的用戶](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target="_blank"} 寫給 [!DNL Commerce] 檔案系統。

1. 將您的網站放入 [維護模式](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target="_blank"}。

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 從 [!DNL Commerce] 項目根目錄，將Channel Manager添加到 `composer.json`。

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. 如果出現提示，請輸入您的 [!DNL Commerce] 帳戶。

   您的公鑰是您的用戶名；你的私鑰是你的密碼。

1. 更新依賴項並安裝擴展。

   ```bash
   composer update magento/channel-manager
   ```

   的 `composer update` 命令僅更新所需的依賴項 [!DNL Channel Manager]。 要更新所有依賴關係，請改用以下命令： `composer update`。

1. 等待Composer完成更新項目依賴項並解決所有錯誤。

1. 驗證模組安裝：

   - 檢查模組狀態。

      ```bash
      bin/magento module:status Magento_SalesChannels
      ```

      示例響應：

      ```terminal
      Module is enabled
      ```

   - 如果未啟用模組，請啟用它。

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. 註冊擴展。

   ```bash
   bin/magento setup:upgrade
   ```

1. 如果出現提示，請重新編譯 [!DNL Commerce] 項目。

   ```bash
   bin/magento setup:di:compile
   ```

1. 清除快取。

   ```bash
   bin/magento cache:clean
   ```

1. 禁用維護模式。

   ```bash
   bin/magento maintenance:disable
   ```

### 在Adobe Commerce上安裝雲基礎架構實例

在向雲實例添加擴展時在開發分支中工作。

有關使用分支的幫助，請參見 [開始建立分支](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted){target="_blank"} 在Adobe Commerce開發人員文檔中。

安裝期間，副檔名(`magento\channel-manager`) [app/etc/config.php](https://devdocs.magento.com/cloud/live/sens-data-over.html#configuration-data){target="_blank"} 的子菜單。 您不需要直接編輯檔案。

1. 在本地工作站上，更改為雲項目根目錄。

1. 建立或簽出開發 [分支](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target="_blank"}。

1. 使用Composer名稱，將擴展添加到 `require` 的下界 `composer.json` 的子菜單。

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. 更新依賴項並安裝擴展。

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   的 `composer update` 命令僅更新所需的依賴項 [!DNL Channel Manager]。 要更新所有依賴關係，請改用以下命令： `composer update`。

1. 添加、提交和推送代碼更改 — 包括對 `composer.lock` 和 `composer.json` 的子菜單。

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m "Install channel manager extension" 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. 構建和部署過程完成後，使用SSH登錄到遠程環境並驗證擴展安裝是否正確。

```bash
   bin/magento module:status Magento_SalesChannels
```

示例響應：

```terminal
Module is enabled
```

如果模組被禁用， [在本地環境中啟用它](https://devdocs.magento.com/cloud/howtos/install-components.html#manage-extensions) 並部署更改。


1. 成功安裝擴展後，請登錄到 [!UICONTROL Admin] 至 [配置Commerce Services連接器](connect.md)。

   >[!NOTE]
   >
   >有關將Channel Manager更新為新版本的說明，請參見 [升級模組和擴展](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target="_blank"}。


## 故障排除

使用以下資訊可解決在Channel Manager安裝過程中發生的錯誤。

### 合成器鍵不正確

如果 [訪問密鑰](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"} 用於驗證到Composer儲存庫的無效，或未連結到 [!DNL MAGE ID] 以前是註冊的 [!DNL Channel Manager] 服務，顯示以下錯誤。

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

1. 驗證auth.json中的憑據是否匹配 [與MAGE ID關聯的鍵](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"} 用於註冊Channel Manager服務。

### 記憶體不足，無法用於PHP

如果系統沒有為PHP分配足夠的記憶體，則會顯示以下錯誤。

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

使用以下任一方法解決記憶體問題：

- [增加PHP的記憶體限制](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit){target="_blank"} in the environment `php.ini` file. Also, verify that the Commerce instance has the [recommended values](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html){target="_blank"} 其他PHP設定。

- 從命令行指定記憶體限制。

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   例如：

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### 缺少視圖

如果您對丟失 `process_catalog_exporter_view` 在Channel Manager安裝過程中，嘗試 [刷新索引器](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target="_blank"}。

```bash
php bin/magento indexer:refresh
```

### 雲部署錯誤

有關將擴展部署到雲的問題，請參見 [擴展部署失敗](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target="_blank"}。
