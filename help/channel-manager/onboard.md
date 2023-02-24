---
title: 板載 [!DNL Channel Manager]
description: '''將您的執行個體連結至 [!DNL Channel Manager] 服務，請完成幾個入門步驟。'
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---


# 板載 [!DNL Channel Manager]

在您完成渠道經理上線流程後，您可以從Adobe Commerce訪問、配置和管理沃爾瑪市場渠道銷售運營。 管道管理員可從 [!UICONTROL Channel Manager] 選項 [!UICONTROL Commerce Admin Marketing] 功能表。

![[!DNL Channel Manager] 選項](assets/channel-manager-admin-view.png)

## 需求

檢閱使用Channel Manager的需求，並收集必要的帳戶資訊和憑證，以下載、安裝及設定擴充功能。

- **[Walmart Marketplace要求](walmart-requirements.md)** — 確認您符合與Channel Manager整合的要求，包括 [設定賣家帳戶](https://sellerhelp.walmart.com/seller/s/guide?article=000008219) 並產生API金鑰以啟用整合。

- **商務帳戶資訊** — 下載和安裝 [!DNL Channel Manager] 要求a [商務帳戶](https://docs.magento.com/user-guide/magento/magento-account.html){target="_blank"}. 您需要帳戶ID和憑證，且擁有 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 例項。

   - **影像ID**-[登入](https://account.magento.com/customer/account/login/) 到 [!DNL Commerce] 帳戶以從 **[!UICONTROL My Account - Magento settings]**.

      ![[!DNL MAGEID] on [!DNL Commerce] 帳戶設定](assets/mageid-my-commerce-account.png)

   - **訪問密鑰 —** 取得要下載的驗證金鑰 [!DNL Commerce] 擴充功能 [!DNL Commerce] 撰寫器存放庫 `([!DNL repo.magento.com]`)。

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      在Adobe Commerce和Magento Open Source專案中，擁有者可以設定 [共用存取](https://docs.magento.com/user-guide/magento/magento-account-share.html) 允許受信任的員工和服務提供商使用所有者或許可證持有者帳戶的憑據下載擴展。

      針對 [!DNL Adobe Commerce] 在雲基礎架構項目上，軟體安裝程式必須具有以下訪問權限 [!DNL Commerce] 例項：

      - 雲端專案的超級使用者存取權
      - 特定環境的管理員存取權
      - an [!DNL Adobe Commerce] 具有存取撰寫器存放庫權限的帳戶

      請參閱 [管理使用者存取](https://devdocs.magento.com/cloud/project/user-admin.html).


- **使用撰寫器和的體驗[!DNL Commerce CLI]** — 請參閱 [一般CLI安裝](https://devdocs.magento.com/extensions/install/){target="_blank"} 有關使用這些工具來安裝和管理擴展的資訊，請參見 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 平台。

- **[[!DNL Amazon Sales Channel] 4.4.2版或更新版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)** — 如果已激活 [!DNL Amazon Sales Channel] 為 [!DNL Commerce] 網站，確認您的 [!DNL Commerce] 安裝之前，platform已安裝4.4.2版或更新版本 [!DNL Channel Manager].

- **[!DNL Inventory Management]Adobe Commerce和Magento Open Source的擴充功能**

   如果您打算使用Channel Manager進行庫存和訂單管理，則必須在Adobe Commerce和Magento Open Source執行個體上安裝並啟用Inventory management擴充功能。 此擴充功能通常會在Adobe Commerce上安裝並預設啟用， [!DNL Magento Open Source] 2.3.x及更新版本。

   如果您從2.2.x升級商務，或您已停用Inventory management，請更新您的安裝以包含必要的模組。 請參閱 [安裝Inventory management](https://devdocs.magento.com/extensions/inventory-management/) 在Adobe Commerce開發人員檔案中。

### 系統需求

- [Adobe Commerce 2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [PHP 7.3 / 7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [撰寫器1.x或更新版本](https://devdocs.magento.com/cloud/reference/cloud-composer.html)
- [[!DNL Amazon Sales Channel] 4.4.2版或更新版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) — 如果已激活 [!DNL Amazon Sales Channel] 為 [!DNL Commerce] 網站，確認您的 [!DNL Commerce] 安裝之前，平台已安裝4.4.2版 [!DNL Channel Manager].
- [[!DNL Inventory Management]](https://devdocs.magento.com/extensions/inventory-management/)

### 支援平台

- Adobe Commerce on Cloud(ECE):2.4.x
- Adobe Commerce內部部署(EE):2.4.x
- Magento Open Source2.4.x

## 入門步驟

1. [設定您的Walmart銷售商帳戶](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp).

1. [安裝 [!DNL Channel Manager] 擴充功能](install.md).

1. [連接到Commerce Services](connect.md) 將Channel Manager與Commerce實例及其他支援服務整合。

1. [連接您的 [!DNL Commerce] 儲存至 [!DNL Walmart Marketplace]](connect-marketplace.md).

1. [完成商店設定](complete-sales-channel-store-setup.md).
