---
title: '安裝 [!DNL Channel Manager]'
description: '''安裝[!DNL Channel Manager] 擴充功能。'
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 31af7107c0b27a236b94f7725b7a107d1027789c
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---


# 安裝 [!DNL Channel Manager]

檢閱 [需求](onboard.md#requirements) 並在安裝Channel Manager之前收集所需資訊。

## 安裝擴充功能

Channel Manager的安裝說明取決於部署在本地還是雲基礎架構上的Adobe Commerce或Magento Open Source。

- 在 [本地實例](#install-on-an-on-premises-instance).

- 在 [[!DNL Adobe Commerce] 在雲基礎架構實例上](#install-adobe-commerce-on-cloud-infrastructure)

兩種方法都要求您使用命令行介面(CLI)。

>[!NOTE]
>
>如需安裝協助 [!DNL Commerce] 使用CLI的軟體，請參見 [一般CLI安裝](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;}。

### 安裝在本地實例上

請依照下列指示進行安裝 [!DNL Channel Manager] 在Adobe Commerce上，並Magento Open Source至內部執行個體。

1. 登入 [!DNL Commerce] 伺服器as a [權限使用者](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/file-system-perms.html){target=&quot;_blank&quot;}要寫入 [!DNL Commerce] 檔案系統。

1. 將您的網站放入 [維護模式](https://devdocs.magento.com/guides/v2.4/install-gde/install/cli/install-cli-subcommands-maint.html){target=&quot;_blank&quot;}。

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 從 [!DNL Commerce] 項目根目錄，將Channel Manager添加到 `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. 如果出現提示，請輸入您 [!DNL Commerce] 帳戶。

   您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

1. 更新相依性並安裝擴充功能。

   ```bash
   composer update magento/channel-manager
   ```

   此 `composer update` 命令僅更新 [!DNL Channel Manager]. 要更新所有依賴項，請改用以下命令： `composer update`.

1. 等待撰寫器完成項目依賴項的更新並解決任何錯誤。

1. 驗證模組安裝：

   - 檢查模組狀態。

      ```bash
      bin/magento module:status Magento_SalesChannels
      ```
      範例回應：

      ```terminal
      Module is enabled
      ```

   - 如果未啟用模組，請啟用它。

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. 註冊擴充功能。

   ```bash
   bin/magento setup:upgrade
   ```

1. 如果出現提示，請重新編譯 [!DNL Commerce] 專案。

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

### 在Adobe Commerce上安裝雲端基礎架構執行個體

將擴充功能新增至雲端例項時，請在開發分支中工作。

如需分支的使用說明，請參閱 [開始建立分支](https://devdocs.magento.com/cloud/env/environments-start.html#getstarted)Adobe Commerce開發人員檔案中的{target=&quot;_blank&quot;}。

安裝期間，擴充功能名稱(`magento\channel-manager`)會自動插入 [app/etc/config.php](https://devdocs.magento.com/cloud/live/sens-data-over.html#configuration-data){target=&quot;_blank&quot;}檔案。 您不需要直接編輯檔案。

1. 在本機工作站上，變更為雲端專案根目錄。

1. 建立或簽出開發 [分支](https://devdocs-beta.magento.com/cloud/env/environments-start.html#getstarted){target=&quot;_blank&quot;}。

1. 使用撰寫器名稱，將擴充功能新增至 `require` 區段 `composer.json` 檔案。

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. 更新相依性並安裝擴充功能。

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   此 `composer update` 命令僅更新 [!DNL Channel Manager]. 要更新所有依賴項，請改用以下命令： `composer update`.

1. 新增、提交和推送程式碼變更 — 包括對 `composer.lock` 和 `composer.json` 檔案。

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m “Install channel manager extension” 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. 建置和部署程式完成後，請使用SSH登入遠端環境，並確認擴充功能已正確安裝。

```bash
   bin/magento module:status Magento_SalesChannels
```

範例回應：

```terminal
Module is enabled
```

如果模組已停用， [在您的本機環境中啟用](https://devdocs.magento.com/cloud/howtos/install-components.html#manage-extensions) 並部署您的變更。


1. 成功安裝擴充功能後，請登入 [!UICONTROL Admin] to [配置Commerce Services Connector](connect.md).

   >[!NOTE]
   >
   >如需將Channel Manager更新至新版本的指示，請參閱 [升級模組和擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html){target=&quot;_blank&quot;}。


## 疑難排解

使用以下資訊解決在Channel Manager安裝過程中發生的錯誤。

### 撰寫器密鑰不正確

若 [存取金鑰](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html)用於驗證到撰寫器儲存庫的{target=&quot;_blank&quot;}無效，或未連結到 [!DNL MAGE ID] 以前註冊 [!DNL Channel Manager] 服務時，會顯示下列錯誤。

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

檢查密鑰配置：

1. 尋找 `auth.json` 檔案：

   ```bash
   $ composer config –global home
   ```

1. 檢視 `auth.json` 檔案。

   ```bash
   $ cat /path/to/auth.json
   ```

1. 確認auth.json中的憑證相符 [與MAGE ID關聯的鍵](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target=&quot;_blank&quot;}用於註冊Channel Manager服務。

### PHP記憶體不足

如果系統沒有為PHP分配足夠的記憶體，則會顯示以下錯誤。

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

使用以下任一方法解決記憶體問題：

- [提高PHP的記憶體限制](https://devdocs.magento.com/cloud/project/magento-app-php-ini.html#increase-php-memory-limit)環境中的{target=&quot;_blank&quot;} `php.ini` 檔案。 此外，確認商務例項具有 [建議值](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html){target=&quot;_blank&quot;}以取得其他PHP設定。

- 從命令行指定記憶體限制。

   ```bash
   $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
   ```

   例如：

   ```bash
   $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
   ```

### 缺少視圖

如果您收到關於遺失的錯誤 `process_catalog_exporter_view` 在Channel Manager安裝期間，嘗試 [刷新索引器](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-index.html#config-cli-subcommands-index-reindex){target=&quot;_blank&quot;}。

```bash
php bin/magento indexer:refresh
```

### 雲部署錯誤

如需將擴充功能部署至雲端的問題，請參閱 [擴充功能部署失敗](https://devdocs.magento.com/cloud/trouble/trouble_comp-deploy-fail.html){target=&quot;_blank&quot;}。
