---
title: '''連接到 [!DNL Commerce] 服務'
description: '''將Channel Manager連接到 [!DNL Commerce] 服務，以啟用資料同步和在 [!DNL Commerce] 實例、Channel Manager和其他支援服務。'
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: 7e7a3e854bbc6062e2d15c1962ddf787451e7275
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# 連接到 [!DNL Commerce] 服務

的 [!DNL Commerce Services Connector] 將Channel Manager服務與Adobe Commerce和Magento Open Source實例整合。 該連接器使資料同步和在 [!DNL Commerce] 實例， [!DNL Channel Manager]以及其他支援服務。

[!DNL Commerce Services Connector] 安裝程式是一次性流程，需要使用 [Adobe CommerceSaaS服務](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;，如 [!DNL Channel Manager]。 [!DNL Live Search], [!DNL Product Recommendations]。 如果已為其他服務配置連接器，請跳過此步驟。

## 要求

- **商業帳戶** — 要在 [!DNL Commerce] 實例，您必須擁有擁有所有者或管理員訪問權限的帳戶 [!DNL Commerce] 平台。

   帳戶所有者和超級用戶可以通過 [!DNL Commerce] 實例或命令行中 [!DNL Commerce] CLI命令 `admin:user:create`。

- **Adobe Commerce生產API密鑰** — 此 [鍵](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}允許API訪問Channel Manager所需的服務。 您需要此密鑰的公共和私有憑據。

>[!TIP]
>
>要提供憑據， [!DNL Commerce] 許可證持有者或帳戶所有者有權 [共用訪問](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;}，或給 [API密鑰](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}到受信任開發人員的憑據。

## 配置 [!DNL Commerce Services Connector]

1. 開啟儲存服務配置。

   - 在管理員中，選擇 **[!UICONTROL Stores]**。

   - 下 *[!UICONTROL Settings]*&#x200B;選中 **[!UICONTROL Configuration]**。

   - 展開 **[!UICONTROL Services]** 選擇 **[!UICONTROL Commerce Services Connector]**。

1. 從您的Adobe Commerce帳戶添加生產API密鑰憑據。

   ![[!DNL Commerce Services Connector] 服務 [!DNL Admin] 視圖](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > 如果 [!DNL Commerce] 實例 [!DNL Adobe Commerce] 服務 [!DNL Live Search] 或 [!DNL Product Recommendations] 已安裝，該介面中將顯示憑據資訊，無需進一步配置。

1. 配置SaaS項目和資料空間，以便Commerce Services可以將資料發送到Channel Manager服務。

   ![[!DNL Commerce Services Connector] SaaS標識符配置 [!DNL Admin] 視圖](assets/commerce-services-connector-saas-config.png)

