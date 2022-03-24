---
title: 連接到Commerce Services
description: 將Channel Manager實例連接到 [!DNL Commerce services] 啟用Commerce實例、Channel Manager和其他支援服務之間的資料同步和通信。
role: User
level: Intermediate
source-git-commit: ec950579a9b2220f9ec106b616779fc3503f3add
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# 連接到Commerce Services

Commerce Services Connector將Channel Manager服務與Adobe Commerce和Magento Open Source實例整合。 該連接器使資料同步和在 [!DNL Commerce] 實例， [!DNL Channel Manager]以及其他支援服務。

Commerce Services Connector安裝程式是使用Adobe所需的一次性流程 [Commerce SaaS服務](https://experienceleague.adobe.com/docs/commerce-merchant-services/user-guides/home.html){target=&quot;_blank&quot;類似 [!DNL Channel Manager]。 [!DNL Live Search], [!DNL Product Recommendations]。 如果已為其他服務配置了連接器，則可以跳過此步驟。

## 先決條件

- **商業帳戶 [管理員訪問](https://docs.magento.com/user-guide/stores/admin.html){target=&quot;_blank&quot;** 到您的Commerce實例** — 帳戶所有者和管理員用戶可以使用 [!DNL Commerce] CLI命令 `admin:user:create`。

- **Adobe Commerce [生產API密鑰](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;** — 啟用對Channel Manager所需服務的API訪問

   要提供憑據，Commerce許可證持有者或帳戶所有者可選擇
   [共用訪問](https://docs.magento.com/user-guide/magento/magento-account-share.html){target=&quot;_blank&quot;}，或給 [API密鑰](https://docs.magento.com/user-guide/system/saas.html#apikey){target=&quot;_blank&quot;}到受信任開發人員的憑據。

## 配置Commerce Services連接器

1. 開啟儲存服務配置。

   - 在管理員中，選擇 [!UICONTROL Stores]。

   - 下 *設定*&#x200B;選中 [!UICONTROL Configuration]。

   - 在 [!UICONTROL Configuration] 頁面，展開 [!UICONTROL Services] 選擇 [!UICONTROL Commerce Services Connector]。

1. 從您的Adobe Commerce帳戶添加生產API密鑰。

   ![[!DNL Commerce Service Connector] 服務 [!DNL Admin] 視圖](assets/commerce-services-connector-admin-service-view.png)


   >[!NOTE]
   >
   > 如果 [!DNL Commerce] 實例 [!DNL Adobe Commerce] 服務 [!DNL Live Search] 或 [!DNL Product Recommendations] 已安裝，該介面中將顯示憑據資訊，無需進一步配置。

1. 配置SaaS項目和資料空間，以便Commerce Services可以將資料發送到Channel Manager服務。

   ![[!DNL Commerce Service Connector] SaaS標識符配置 [!DNL Admin] 視圖](assets/commerce-services-connector-saas-config.png)

