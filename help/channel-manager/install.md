---
title: '安裝 [!DNL Channel Manager]'
description: '安裝[!DNL Channel Manager]擴充功能。'
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 1e74150e6ac88dbabb2e4bbb2fa2f243072eb03f
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# 安裝[!DNL Channel Manager]

檢閱[需求](onboard.md#requirements)，並收集必要的資訊，然後再安裝Channel Manager。

## 安裝擴充功能

Channel Manager的安裝指示取決於Adobe Commerce或Magento Open Source是部署在內部部署還是部署在雲端基礎結構上。

- 安裝在[內部部署執行個體](#install-on-an-on-premises-instance)上。

- 在雲端基礎結構執行個體](#install-adobe-commerce-on-cloud-infrastructure)上的[[!DNL Adobe Commerce] 上安裝

這兩種方法都需要您使用命令列介面(CLI)。

>[!NOTE]
>
>如需使用CLI安裝[!DNL Commerce]軟體的說明，請參閱[安裝擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)。

### 安裝在內部部署執行個體上

使用這些指示在Adobe Commerce上安裝[!DNL Channel Manager]並Magento Open Source到內部部署執行個體。

1. 以[使用者身分登入[!DNL Commerce]伺服器，並擁有寫入[!DNL Commerce]檔案系統的許可權](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html)。

1. 將您的網站置於[維護模式](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html)。

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 從[!DNL Commerce]專案根目錄，將頻道管理員新增至`composer.json`。

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. 如果出現提示，請輸入您[!DNL Commerce]帳戶的存取金鑰。

   您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

1. 更新相依性並安裝擴充功能。

   ```bash
   composer update magento/channel-manager
   ```

   `composer update`命令只會更新[!DNL Channel Manager]所需的相依性。 若要更新所有相依性，請改用此命令： `composer update`。

1. 等待Composer完成更新專案相依性並解決任何錯誤。

1. 驗證模組安裝：

   - 檢查模組狀態。

     ```bash
     bin/magento module:status Magento_SalesChannels
     ```

     範例回應：

     ```
     Module is enabled
     ```

   - 如果未啟用此模組，請啟用它。

   ```bash
   bin/magento module:enable Magento_SalesChannels
   ```

1. 註冊擴充功能。

   ```bash
   bin/magento setup:upgrade
   ```

1. 如果出現提示，請重新編譯您的[!DNL Commerce]專案。

   ```bash
   bin/magento setup:di:compile
   ```

1. 清除快取。

   ```bash
   bin/magento cache:clean
   ```

1. 停用維護模式。

   ```bash
   bin/magento maintenance:disable
   ```

### 在雲端基礎結構執行個體上的Adobe Commerce上安裝

將擴充功能新增至雲端例項時，請在開發分支中工作。

如需使用分支的協助，請參閱&#x200B;_雲端基礎結構上的Commerce指南_&#x200B;中的[開始建立分支](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html)。

在安裝期間，擴充功能名稱(`magento\channel-manager`)會自動插入[app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html)檔案。 您不需要直接編輯檔案。

1. 在本機工作站上，變更至雲端專案根目錄。

1. 建立或簽出開發[分支](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html)。

1. 使用撰寫器名稱，將副檔名新增至`composer.json`檔案的`require`區段。

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. 更新相依性並安裝擴充功能。

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   `composer update`命令只會更新[!DNL Channel Manager]所需的相依性。 若要更新所有相依性，請改用此命令： `composer update`。

1. 新增、認可及推播程式碼變更 — 包含對`composer.lock`和`composer.json`檔案的變更。

   ```bash
   $ git add -A
   ```

   ```bash
   $ git commit -m "Install channel manager extension" 
   ```

   ```bash
   $ git push origin <branch-name>
   ```

1. 建置和部署程式完成後，請使用SSH登入遠端環境，並確認擴充功能是否已正確安裝。

```bash
   bin/magento module:status Magento_SalesChannels
```

範例回應：

```
Module is enabled
```

如果模組已停用，請[在本機環境中啟用它](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html)，並部署您的變更。


1. 成功安裝擴充功能後，請登入[!UICONTROL Admin]以[設定Commerce服務聯結器](connect.md)。

   >[!NOTE]
   >
   >如需將Channel Manager更新為新版本的指示，請參閱[升級模組與擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html)。


## 疑難排解

使用下列資訊來解決Channel Manager安裝過程中發生的錯誤。

### 不正確的撰寫器索引鍵

如果用於驗證撰寫器存放庫的[存取金鑰](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html)無效，或未連結至用於註冊[!DNL Channel Manager]服務的[!DNL MAGE ID]，則會顯示下列錯誤。

```
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

檢查金鑰組態：

1. 尋找`auth.json`檔案的位置：

   ```bash
   $ composer config –global home
   ```

1. 檢視`auth.json`檔案。

   ```bash
   $ cat /path/to/auth.json
   ```

1. 請確認auth.json中的認證符合用來註冊Channel Manager服務的MAGE ID](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html)所關聯的[金鑰。

### PHP的記憶體不足

如果系統沒有為PHP分配足夠的記憶體，則會顯示以下錯誤。

```
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

請使用下列其中一種方法來解決記憶體問題：

- [增加環境`php.ini`檔案中PHP](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html)的記憶體限制。 此外，請確認Commerce執行個體具有其他PHP設定的[建議值](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)。

- 從命令列指定記憶體限制。

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  例如：

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### 缺少檢視

如果在頻道管理員安裝期間發生有關遺失`process_catalog_exporter_view`的錯誤，請嘗試[重新整理索引子](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html)。

```bash
php bin/magento indexer:refresh
```

### 雲端部署錯誤

如需將擴充功能部署至雲端時發生的問題，請參閱[擴充功能部署失敗](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html)。
