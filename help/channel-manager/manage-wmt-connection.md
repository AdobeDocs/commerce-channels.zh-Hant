---
title: 管理Walmart Marketplace連線
description: '''更新API認證以授權[DNL！ Commerce]商店檢視和 [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] 產品清單，並同步化存貨、價格、訂單及運送資料，介於 [!DNL Commerce] 還有沃爾瑪。'
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# 對應出貨承運商

在您之前 [處理訂單出貨](process-orders.md#ship-an-order) 的 [!DNL Walmart Marketplace] 訂單，將Walmart偏好的運送公司對應至中的對應承運商 [!DNL Commerce] 以便運送資料可以同步到 [!DNL Walmart] 和 [!DNL Commerce].

未對應至偏好電信業者的商務電信業者會標籤為 *[!UICONTROL Other Carrier]* 於 [!DNL Walmart].

**必要條件**

檢閱 [沃爾瑪規定](walmart-requirements.md) 針對 [!DNL Marketplace Seller account].

## 更新連線認證

1. 在 [!UICONTROL Listings] 銷售管道商店的頁面，選取 **[!UICONTROL Channel Settings]**.

1. 開啟 **[!UICONTROL Channel Settings]**，選取 **[!UICONTROL Walmart Connection]**.

1. 若要修改認證，請選取 **[!UICONTROL Change Credentials]**

   ![更新Walmart API認證以授權連線](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. 輸入 **[!UICONTROL Walmart Client ID]** 和 **[!UICONTROL Walmart Client Secret]**.

1. 選取 **[!UICONTROL Save]** 以套用組態。
