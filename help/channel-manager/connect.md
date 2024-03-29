---
title: '''連線到 [!DNL Commerce] 服務'
description: '''連線管道管理員 [!DNL Commerce] 服務，啟用資料同步化及以下專案之間的通訊： [!DNL Commerce] 執行個體、管道管理員和其他支援服務。'
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# 連線到 [!DNL Commerce] 服務

此 [!DNL Commerce Services Connector] 整合Channel Manager服務與Adobe Commerce和Magento Open Source執行個體。 聯結器會啟用資料同步化以及 [!DNL Commerce] 例項， [!DNL Channel Manager]和其他支援服務。

[!DNL Commerce Services Connector] 安裝程式需要一次性使用 [Adobe Commerce SaaS服務](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) 例如 [!DNL Channel Manager]， [!DNL Live Search]、和 [!DNL Product Recommendations]. 如果您已經為另一個服務設定了聯結器，請略過此步驟。

## 需求

- **Commerce帳戶** — 若要安裝軟體至 [!DNL Commerce] 執行個體，您必須擁有擁有擁有者或管理員存取權的帳戶， [!DNL Commerce] 平台。

  帳戶擁有者和超級使用者可以從以下位置建立管理員帳戶： [!DNL Commerce] 例項或從命令列使用 [!DNL Commerce] CLI命令 `admin:user:create`.

- **Adobe Commerce生產API金鑰** — 這個 [key](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey) 啟用API存取通道管理員所需的服務。 您需要此金鑰的公開和私人認證。

>[!TIP]
>
>若要提供認證，請 [!DNL Commerce] 授權擁有者或帳戶擁有者有選項可以 [共用存取權](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)，或賦予 [API金鑰](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html) 認證給信任的開發人員。

## 設定 [!DNL Commerce Services Connector]

1. 開啟Store Services設定。

   - 在「管理員」中，選取 **[!UICONTROL Stores]**.

   - 在 *[!UICONTROL Settings]*，選取 **[!UICONTROL Configuration]**.

   - 展開 **[!UICONTROL Services]** 並選取 **[!UICONTROL Commerce Services Connector]**.

1. 從您的Adobe Commerce帳戶新增生產API金鑰認證。

   ![[!DNL Commerce Services Connector] 中的服務 [!DNL Admin] 檢視](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > 若您的 [!DNL Commerce] 執行個體有其他 [!DNL Adobe Commerce] 服務如 [!DNL Live Search] 或 [!DNL Product Recommendations] 已安裝，認證資訊會顯示在介面中，不需要進一步設定。

1. 設定SaaS專案和資料空間，讓Commerce Services可以將資料傳送至Channel Manager服務。

   ![[!DNL Commerce Services Connector] 中的SaaS識別碼設定 [!DNL Admin] 檢視](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}

