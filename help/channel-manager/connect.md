---
title: '連接到 [!DNL Commerce] 服務'
description: '''將Channel Manager連接到 [!DNL Commerce] 使資料同步和通信在 [!DNL Commerce] 例項、渠道管理器和其他支援服務。'
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---


# 連線至 [!DNL Commerce] 服務

此 [!DNL Commerce Services Connector] 整合了Channel Manager服務與Adobe Commerce和Magento Open Source執行個體。 該連接器可實現資料同步以及 [!DNL Commerce] 例項， [!DNL Channel Manager]，以及其他支援服務。

[!DNL Commerce Services Connector] 設定是使用的一次性程式 [Adobe Commerce SaaS服務](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target="_blank"} 例如 [!DNL Channel Manager], [!DNL Live Search]，和 [!DNL Product Recommendations]. 如果您已配置其他服務的連接器，請跳過此步驟。

## 需求

- **商務帳戶** — 在上安裝軟體 [!DNL Commerce] 例項，您必須擁有擁有者或管理員存取權的帳戶 [!DNL Commerce] 平台。

   帳戶擁有者和超級使用者可以從 [!DNL Commerce] 執行個體或從命令列使用 [!DNL Commerce] CLI命令 `admin:user:create`.

- **Adobe Commerce生產API金鑰** — 此 [key](https://docs.magento.com/user-guide/system/saas.html#apikey){target="_blank"} 可讓API存取管道管理員所需的服務。 您需要此金鑰的公開和私人憑證。

>[!TIP]
>
>若要提供憑證，請 [!DNL Commerce] 許可證持有者或帳戶擁有者可以選擇 [共用存取](https://docs.magento.com/user-guide/magento/magento-account-share.html){target="_blank"}, or give the [API Key](https://docs.magento.com/user-guide/system/saas.html#apikey){target="_blank"} 認證給受信任的開發人員。

## 設定 [!DNL Commerce Services Connector]

1. 開啟「商店服務」設定。

   - 在管理員中，選取 **[!UICONTROL Stores]**.

   - 在 *[!UICONTROL Settings]*，選取 **[!UICONTROL Configuration]**.

   - 展開 **[!UICONTROL Services]** 選取 **[!UICONTROL Commerce Services Connector]**.

1. 從您的Adobe Commerce帳戶新增生產API金鑰憑證。

   ![[!DNL Commerce Services Connector] 服務 [!DNL Admin] 檢視](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > 若您的 [!DNL Commerce] 實例 [!DNL Adobe Commerce] 服務贊 [!DNL Live Search] 或 [!DNL Product Recommendations] 已安裝，憑據資訊將顯示在介面中，無需進一步配置。

1. 配置SaaS項目和資料空間，以便Commerce Services可以將資料發送到Channel Manager服務。

   ![[!DNL Commerce Services Connector] SaaS標識符配置 [!DNL Admin] 檢視](assets/commerce-services-connector-saas-config.png)

