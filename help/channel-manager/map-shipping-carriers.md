---
title: 對應出貨承運商
description: '對應屬性以符合[DNL！ Commerce]產品至現有 [!DNL Walmart Marketplace] 列出及同步資料介於 [!DNL Channel Manager] 和 [!DNL Walmart].'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# 對應出貨承運商

在您之前 [處理訂單出貨](process-orders.md#ship-an-order) 的 [!DNL Walmart Marketplace] 訂單，將Walmart偏好的運送公司對應至中的對應承運商 [!DNL Commerce] 以便運送資料可以同步到 [!DNL Walmart] 和 [!DNL Commerce].

未對應至偏好電信業者的商務電信業者會標籤為 *[!UICONTROL Other Carrier]* 於 [!DNL Walmart].

**必要條件**

在對映出貨承運商之前，請先完成下列作業：

1. 檢閱 [準時交貨的承運商方法與運送最佳實務](https://sellerhelp.walmart.com/s/guide?article=000009473) 的 [!DNL Walmart Marketplace].

1. 驗證 [[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html) 和 [[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html) 設定 [!DNL Commerce] 存放區以確保您已針對最佳化設定 [!DNL Walmart Marketplace sales].

## 對應出貨承運商

1. 從 **[!UICONTROL Listings]** 或 **[!UICONTROL Orders]** 頁面，選取 **[!UICONTROL Channel Settings]**.

1. 開啟 **[!UICONTROL Channel Settings]**，選取 **[!UICONTROL Shipping Carriers]**.

   ![對應出貨承運商](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. 針對每個 [!DNL Walmart] 列出偏好的電信業者，選取 [!DNL Commerce] 電信業者可用時，從下拉式清單取得電信業者名稱。

1. 選取 **[!UICONTROL Save]** 以套用組態。

