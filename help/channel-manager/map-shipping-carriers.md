---
title: 對應出貨承運商
description: '''對應屬性以符合[DNL！ Commerce]產品到現有的 [!DNL Walmart Marketplace] 清單，並在 [!DNL Channel Manager] 和 [!DNL Walmart]之間同步資料。'
role: Admin
feature: Sales Channels, Configuration, Shipping/Delivery
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# 對應出貨承運商

在您[處理[!DNL Walmart Marketplace]個訂單的訂單出貨](process-orders.md#ship-an-order)之前，請將Walmart偏好的出貨承運商對應至[!DNL Commerce]中對應的承運商，以便在[!DNL Walmart]與[!DNL Commerce]之間同步出貨資料。

未對應到慣用電信業者的Commerce電信業者在[!DNL Walmart]上標示為&#x200B;*[!UICONTROL Other Carrier]*。

**必要條件**

在對映出貨承運商之前，請先完成下列作業：

1. 檢閱[!DNL Walmart Marketplace]的準時傳遞](https://sellerhelp.walmart.com/s/guide?article=000009473)的[電信業者方法和運送最佳實務。

1. 驗證[!DNL Commerce]存放區中的[[!UICONTROL Shipping Carrier]](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/delivery/shipping-carriers/carriers.html)與[[!UICONTROL Shipping Settings]](https://experienceleague.adobe.com/docs/commerce-admin/config/sales/shipping-settings.html)設定，以確定您已最佳化[!DNL Walmart Marketplace sales]的設定。

## 對應出貨承運商

1. 從&#x200B;**[!UICONTROL Listings]**&#x200B;或&#x200B;**[!UICONTROL Orders]**&#x200B;頁面，選取&#x200B;**[!UICONTROL Channel Settings]**。

1. 在&#x200B;**[!UICONTROL Channel Settings]**&#x200B;上，選取&#x200B;**[!UICONTROL Shipping Carriers]**。

   ![對應運送公司](assets/map-shipping-carriers.png){width="600" zoomable="yes"}

1. 對於列出的每個[!DNL Walmart]慣用電信業者，如果該電信業者可用，請從下拉式清單中選取[!DNL Commerce]電信業者名稱。

1. 選取&#x200B;**[!UICONTROL Save]**&#x200B;以套用組態。

