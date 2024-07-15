---
title: 內建 [!DNL Channel Manager]
description: '完成一些上線步驟，將您的執行個體連結至 [!DNL Channel Manager] 服務。'
level: Intermediate
role: Leader, Admin, Developer
feature: Sales Channels, Install
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---


# 上線[!DNL Channel Manager]

在您完成「銷售通路管理員」上線流程後，即可從Adobe Commerce存取、設定及管理Walmart Marketplace的銷售通路營運。 管道管理員可從[!UICONTROL Commerce Admin Marketing]功能表上的[!UICONTROL Channel Manager]選項取得。

管理檢視中的![[!DNL Channel Manager]選項](assets/channel-manager-admin-view.png){width="500"}

## 需求

檢閱使用Channel Manager的需求，並收集下載、安裝和設定擴充功能所需的帳戶資訊和認證。

- **[Walmart Marketplace需求](walmart-requirements.md)** — 確認您符合與「通路管理員」整合的需求，包括[設定您的賣家帳戶](https://sellerhelp.walmart.com/seller/s/guide?article=000008219)並產生API金鑰以啟用整合。

- **Commerce帳戶資訊** — 下載和安裝[!DNL Channel Manager]需要[Commerce帳戶](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-create.html)。 您需要帳戶ID和認證，且擁有[!DNL Adobe Commerce]或[!DNL Magento Open Source]執行個體的擁有者或管理員存取權。

   - **影像識別碼**-[登入](https://account.magento.com/customer/account/login/)至[!DNL Commerce]帳戶，以從&#x200B;**[!UICONTROL My Account - Magento settings]**&#x200B;取得識別碼。

     [!DNL Commerce]帳戶設定上的![[!DNL MAGEID]](assets/mageid-my-commerce-account.png){width="250"}

   - **存取金鑰 —**&#x200B;取得驗證金鑰，以從[!DNL Commerce] Composer存放庫`([!DNL repo.magento.com]`下載[!DNL Commerce]延伸模組。

     ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png){width="400"}

     在Adobe Commerce和Magento Open Source專案中，擁有者可以設定[共用存取](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)，以允許受信任的員工和服務提供者使用擁有者或授權擁有者帳戶的認證來下載擴充功能。

     對於雲端基礎結構專案上的[!DNL Adobe Commerce]，軟體安裝程式必須具備對[!DNL Commerce]執行個體的下列存取權：

      - 雲端專案的超級使用者存取權
      - 管理員存取特定環境
      - 具有存取撰寫器存放庫許可權的[!DNL Adobe Commerce]帳戶

     請參閱&#x200B;*雲端基礎結構上的Commerce指南*&#x200B;中的[管理使用者存取權](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/project/user-access.html)。

- **使用撰寫器和[!DNL Commerce CLI]**&#x200B;的經驗 — 請參閱&#x200B;*安裝指南*&#x200B;中的[安裝擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html)，瞭解如何使用這些工具在[!DNL Adobe Commerce]或[!DNL Magento Open Source]平台上安裝和管理擴充功能。

- **[[!DNL Amazon Sales Channel] 版本4.4.2或更新版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html)** — 如果您為[!DNL Commerce]網站啟動[!DNL Amazon Sales Channel]，請在安裝[!DNL Channel Manager]之前，先確認您的[!DNL Commerce]平台已安裝4.4.2或更新版本。

- 適用於Adobe Commerce和Magento Open Source的&#x200B;**[!DNL Inventory Management]延伸模組**

  如果您打算使用「通路管理員」進行存貨與訂單管理，則必須在Adobe Commerce與Magento Open Source執行個體上安裝並啟用Inventory management擴充功能。 一般而言，此擴充功能會在Adobe Commerce及[!DNL Magento Open Source] 2.3.x和更新版本上依預設安裝並啟用。

  如果您從2.2.x升級Commerce，或您已停用Inventory management，請更新您的安裝以包含必要的模組。 請參閱&#x200B;*Inventory management指南*&#x200B;中的[安裝Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)。

### 系統需求

- [Adobe Commerce 2.4.x](https://experienceleague.adobe.com/docs/commerce-operations/release/versions.html)
- [PHP 7.3 / 7.4](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/php-settings.html)
- [Composer 1.x或更新版本](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/develop/overview.html)
- [[!DNL Amazon Sales Channel] 版本4.4.2或更新版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) — 如果您已經啟動[!DNL Commerce]網站的[!DNL Amazon Sales Channel]，請在安裝[!DNL Channel Manager]之前，先確認您的[!DNL Commerce]平台已安裝4.4.2版。
- [[!DNL Inventory Management]](https://experienceleague.adobe.com/docs/commerce-admin/inventory/get-started/install-update.html)

### 支援平台

- 雲端上的Adobe Commerce (ECE) ： 2.4.x
- Adobe Commerce內部部署(EE) ： 2.4.x
- Magento Open Source2.4.x

## 入門步驟

1. [設定您的沃爾瑪賣家帳戶](https://seller.walmart.com/signup?q=&amp;origin=solution_provider&amp;src=0014M00001zivMp)。

1. [安裝 [!DNL Channel Manager] 擴充功能](install.md)。

1. [連線至Commerce Services](connect.md)以整合管道管理員與Commerce執行個體及其他支援服務。

1. [將您的 [!DNL Commerce] 存放區連線至 [!DNL Walmart Marketplace]](connect-marketplace.md)。

1. [完成商店設定](complete-sales-channel-store-setup.md)。
