---
title: '''安裝 [!DNL Channel Manager]『'
description: '安裝[!DNL Channel Manager] 副檔名。'
role: Admin, Developer
feature: Sales Channels, Install
exl-id: cb593ebd-f077-4a79-a661-bedf4cc70f97
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---


# 安裝 [!DNL Channel Manager]

檢閱 [需求](onboard.md#requirements) 並收集必要的資訊，然後再安裝Channel Manager。

## 安裝擴充功能

Channel Manager的安裝指示取決於Adobe Commerce或Magento Open Source是部署在內部部署還是部署在雲端基礎結構上。

- 安裝在 [內部部署執行個體](#install-on-an-on-premises-instance).

- 安裝在 [[!DNL Adobe Commerce] 在雲端基礎結構執行個體上](#install-adobe-commerce-on-cloud-infrastructure)

這兩種方法都需要您使用命令列介面(CLI)。

>[!NOTE]
>
>如需安裝的協助 [!DNL Commerce] 使用CLI的軟體，請參閱 [安裝擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

### 安裝在內部部署執行個體上

使用這些指示來安裝 [!DNL Channel Manager] Adobe Commerce和Magento Open Source至內部部署執行個體上。

1. 登入 [!DNL Commerce] server as a [具有許可權的使用者](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/file-system/configure-permissions.html) 以寫入 [!DNL Commerce] 檔案系統。

1. 將您的網站放入 [維護模式](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/maintenance-mode.html).

   ```bash
   $ bin/magento maintenance:enable
   ```

1. 從 [!DNL Commerce] 專案根目錄，新增通道管理員至 `composer.json`.

   ```bash
    composer require magento/channel-manager --no-update
   ```

1. 如果出現提示，請輸入 [!DNL Commerce] 帳戶。

   您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

1. 更新相依性並安裝擴充功能。

   ```bash
   composer update magento/channel-manager
   ```

   此 `composer update` 命令只會更新所需的相依性 [!DNL Channel Manager]. 若要更新所有相依性，請改用此命令： `composer update`.

1. 等待Composer完成更新專案相依性並解決任何錯誤。

1. 驗證模組安裝：

   - 檢查模組狀態。

     ```bash
     bin/magento module:status Magento_SalesChannels
     ```

     範例回應：

     ```terminal
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

1. 如果出現提示，請重新編譯 [!DNL Commerce] 專案。

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

如需使用分支的說明，請參閱 [開始建立分支](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html) 在 _雲端基礎結構上的Commerce指南_.

在安裝期間，擴充功能名稱(`magento\channel-manager`)會自動插入 [app/etc/config.php](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/store-settings.html) 檔案。 您不需要直接編輯檔案。

1. 在本機工作站上，變更至雲端專案根目錄。

1. 建立或簽出開發 [分支](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/cli-branches.html).

1. 使用撰寫器名稱，將擴充功能新增至 `require` 的區段 `composer.json` 檔案。

   ```bash
   composer require magento/module-sales-channels-extension --no-update
   ```

1. 更新相依性並安裝擴充功能。

   ```bash
   composer update magento/module-sales-channels-extension
   ```

   此 `composer update` 命令只會更新所需的相依性 [!DNL Channel Manager]. 若要更新所有相依性，請改用此命令： `composer update`.

1. 新增、提交和推送程式碼變更 — 包含對兩者的變更 `composer.lock` 和 `composer.json` 檔案。

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

```terminal
Module is enabled
```

如果模組已停用， [在您的本機環境中啟用它](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure-store/extensions.html) 並部署您的變更。


1. 成功安裝擴充功能後，請登入 [!UICONTROL Admin] 至 [設定Commerce服務聯結器](connect.md).

   >[!NOTE]
   >
   >如需將Channel Manager更新至新版本的指示，請參閱 [升級模組和擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/upgrade-guide/modules/upgrade.html).


## 疑難排解

使用下列資訊來解決Channel Manager安裝過程中發生的錯誤。

### 不正確的撰寫器索引鍵

如果 [存取金鑰](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) 用於向Composer存放庫驗證無效，或未連結到 [!DNL MAGE ID] 用於註冊 [!DNL Channel Manager] 服務，下列錯誤會顯示。

```terminal
Could not find a matching version of package magento/channel-manager. Check the package spelling, your version constraint and that the package is available in a stability which matches your minimum-stability (stable).
```

檢查金鑰組態：

1. 尋找的位置 `auth.json` 檔案：

   ```bash
   $ composer config –global home
   ```

1. 檢視 `auth.json` 檔案。

   ```bash
   $ cat /path/to/auth.json
   ```

1. 驗證auth.json中的認證是否相符 [與影像ID相關聯的金鑰](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html) 用於註冊Channel Manager服務。

### PHP的記憶體不足

如果系統沒有為PHP分配足夠的記憶體，則會顯示以下錯誤。

```terminal
Fatal error: Allowed memory size of 2146435072 bytes exhausted (tried to allocate 4096 bytes) in phar:///usr/local/bin/composer/src/Composer/DependencyResolver/RuleWatchGraph.php on line 52
```

請使用下列其中一種方法來解決記憶體問題：

- [增加PHP的記憶體限制](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/php-settings.html) 在環境中 `php.ini` 檔案。 此外，確認商務例項具有 [建議值](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html) 用於其他PHP設定。

- 從命令列指定記憶體限制。

  ```bash
  $ php -d memory_limit=-1 \[path to composer]/composer require magento/payment-services.
  ```

  例如：

  ```bash
  $ php-d memory_limit=-1 vendor/bin/composer require magento/channel-manager
  ```

### 缺少檢視

如果您收到有關遺失的錯誤 `process_catalog_exporter_view` 在安裝通道管理員期間，請嘗試 [重新整理索引子](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/manage-indexers.html).

```bash
php bin/magento indexer:refresh
```

### 雲端部署錯誤

如需將擴充功能部署至雲端的問題，請參閱 [擴充功能部署失敗](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/deploy/recover-failed-deployment.html).
