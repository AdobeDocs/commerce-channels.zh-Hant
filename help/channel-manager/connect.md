---
title: 連接到 [!DNL Commerce] 服務
description: 將Channel Manager連接到 [!DNL Commerce] 服務，以啟用資料同步和在 [!DNL Commerce] 實例、 Channel Manager和其他支援服務。
role: User
level: Intermediate
exl-id: 97da2142-ecef-44dc-91d8-5dc55c713d31
source-git-commit: aaab7aa7feb05264c24386e62193564dc5ae8fe3
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---


# 連接到 [!DNL Commerce] 服務

Commerce Services Connector將Channel Manager服務與Adobe Commerce和Magento Open Source實例整合。 該連接器使資料同步和在 [!DNL Commerce] 實例， [!DNL Channel Manager]以及其他支援服務。

Commerce Services Connector安裝程式是使用Adobe所需的一次性流程 [Commerce SaaS服務](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;類似 [!DNL Channel Manager]。 [!DNL Live Search], [!DNL Product Recommendations]。 如果已為其他服務配置連接器，請跳過此步驟。

## 要求

- **商業帳戶** — 要在Commerce實例上安裝軟體，您必須擁有對Commerce平台具有「所有者」或「管理員」訪問權限的帳戶。

   帳戶所有者和超級用戶可以使用 [!DNL Commerce] CLI命令 `admin:user:create`。

- **Adobe Commerce生產API密鑰** — 此 [鍵](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}允許API訪問Channel Manager所需的服務。 您需要此密鑰的公共和私有憑據。

>[!TIP]
>
>要提供憑據，Commerce許可證持有者或帳戶所有者可選擇 [共用訪問](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;}，或給 [API密鑰](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}到受信任開發人員的憑據。

## 配置Commerce Services連接器

1. 開啟儲存服務配置。

   - 在管理員中，選擇 **[!UICONTROL Stores]**。

   - 下 *[!UICONTROL Settings]*&#x200B;選中 **[!UICONTROL Configuration]**。

   - 展開 **[!UICONTROL Services]** 選擇 **[!UICONTROL Commerce Services Connector]**。

1. 從您的Adobe Commerce帳戶添加生產API密鑰憑據。

   ![[!DNL Commerce Service Connector] 服務 [!DNL Admin] 視圖](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > 如果 [!DNL Commerce] 實例 [!DNL Adobe Commerce] 服務 [!DNL Live Search] 或 [!DNL Product Recommendations] 已安裝，該介面中將顯示憑據資訊，無需進一步配置。

1. 配置SaaS項目和資料空間，以便Commerce Services可以將資料發送到Channel Manager服務。

   ![[!DNL Commerce Service Connector] SaaS標識符配置 [!DNL Admin] 視圖](assets/commerce-services-connector-saas-config.png)

