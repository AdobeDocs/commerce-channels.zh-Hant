---
title: '連線到 [!DNL Commerce] 服務'
description: '將頻道管理員連線到 [!DNL Commerce] 服務，以啟用 [!DNL Commerce] 執行個體、頻道管理員和其他支援服務之間的資料同步和通訊。'
role: Admin, Developer
level: Intermediate
feature: Sales Channels, Install, Integration
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 連線到[!DNL Commerce]服務

[!DNL Commerce Services Connector]整合Channel Manager服務與Adobe Commerce和Magento Open Source執行個體。 聯結器會啟用[!DNL Commerce]執行個體、[!DNL Channel Manager]與其他支援服務之間的資料同步和通訊。

[!DNL Commerce Services Connector]安裝程式是使用[Adobe Commerce SaaS服務](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html) （例如[!DNL Channel Manager]、[!DNL Live Search]和[!DNL Product Recommendations]）所需的一次性程式。 如果您已經為另一個服務設定了聯結器，請略過此步驟。

## 需求

- **Commerce帳戶** — 若要在[!DNL Commerce]執行個體上安裝軟體，您必須擁有擁有[!DNL Commerce]平台擁有者或管理員存取權的帳戶。

  帳戶擁有者和超級使用者可以使用[!DNL Commerce] CLI命令`admin:user:create`，從[!DNL Commerce]執行個體或命令列建立管理員帳戶。

- **Adobe Commerce生產API金鑰** — 此[金鑰](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html#genapikey)可讓API存取頻道管理員所需的服務。 您需要此金鑰的公開和私人認證。

>[!TIP]
>
>若要提供認證，[!DNL Commerce]授權擁有者或帳戶擁有者可選擇[共用存取權](https://experienceleague.adobe.com/docs/commerce-admin/start/commerce-account/commerce-account-share.html)，或將[API金鑰](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/integration-services/saas.html)認證提供給信任的開發人員。

## 設定[!DNL Commerce Services Connector]

1. 開啟Store Services設定。

   - 從Admin中，選取&#x200B;**[!UICONTROL Stores]**。

   - 在&#x200B;*[!UICONTROL Settings]*&#x200B;下，選取&#x200B;**[!UICONTROL Configuration]**。

   - 展開&#x200B;**[!UICONTROL Services]**&#x200B;並選取&#x200B;**[!UICONTROL Commerce Services Connector]**。

1. 從您的Adobe Commerce帳戶新增生產API金鑰認證。

   [!DNL Admin]檢視中的![[!DNL Commerce Services Connector]服務](assets/commerce-services-connector-admin-service-view.png){width="600" zoomable="yes"}


   >[!NOTE]
   >
   > 如果您的[!DNL Commerce]執行個體已安裝其他[!DNL Adobe Commerce]服務（例如[!DNL Live Search]或[!DNL Product Recommendations]），則認證資訊會顯示在介面中，而不需要進一步的設定。

1. 設定SaaS專案和資料空間，讓Commerce Services能夠將資料傳送至Channel Manager服務。

   在[!DNL Admin]檢視](assets/commerce-services-connector-saas-config.png){width="600" zoomable="yes"}中的![[!DNL Commerce Services Connector] SaaS識別碼設定

