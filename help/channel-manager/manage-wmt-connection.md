---
title: 管理Walmart Marketplace連線
description: '''更新API認證以授權[DNL！ Commerce]商店檢視和 [!DNL Walmart Marketplace]. The connection is required to connect [!DNL Commerce] 產品清單，並在 [!DNL Commerce] 和Walmart之間同步化存貨、價格、訂單和運送資料。'
role: Admin, Developer
feature: Sales Channels, Configuration, Shipping/Delivery, Integration
exl-id: 817b1b58-a57e-4c8d-b08f-1ce3bec15bc3
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# 對應出貨承運商

在您[處理[!DNL Walmart Marketplace]個訂單的訂單出貨](process-orders.md#ship-an-order)之前，請將Walmart偏好的出貨承運商對應至[!DNL Commerce]中對應的承運商，以便在[!DNL Walmart]與[!DNL Commerce]之間同步出貨資料。

未對應到慣用電信業者的Commerce電信業者在[!DNL Walmart]上標示為&#x200B;*[!UICONTROL Other Carrier]*。

**必要條件**

檢閱[!DNL Marketplace Seller account]的[沃爾瑪需求](walmart-requirements.md)。

## 更新連線認證

1. 在Sales Channel商店的[!UICONTROL Listings]頁面上，選取&#x200B;**[!UICONTROL Channel Settings]**。

1. 在&#x200B;**[!UICONTROL Channel Settings]**&#x200B;上，選取&#x200B;**[!UICONTROL Walmart Connection]**。

1. 若要修改認證，請選取&#x200B;**[!UICONTROL Change Credentials]**

   ![更新Walmart API認證以授權連線](assets/update-connection-credentials.png){width="700" zoomable="yes"}

1. 輸入&#x200B;**[!UICONTROL Walmart Client ID]**&#x200B;和&#x200B;**[!UICONTROL Walmart Client Secret]**。

1. 選取&#x200B;**[!UICONTROL Save]**&#x200B;以套用組態。
