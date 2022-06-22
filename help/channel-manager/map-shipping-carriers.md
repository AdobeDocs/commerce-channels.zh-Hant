---
title: 映射運輸承運人
description: '''映射匹配的屬性[DNL! Commerce]產品到現有 [!DNL Walmart Marketplace] 清單和同步資料 [!DNL Channel Manager] 和 [!DNL Walmart]'''
exl-id: 98c8d3f6-f129-43c6-920c-d9c36b0e4a40
source-git-commit: 638ba8c595652e66aa5f15f5207855c6d2b872d7
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---


# 映射運輸承運人

在你之前 [處理訂單發運](process-orders.md#ship-an-order) 為 [!DNL Walmart Marketplace] 訂單，將沃爾瑪青睞的貨運公司映射到 [!DNL Commerce] 這樣，運輸資料就可以在 [!DNL Walmart] 和 [!DNL Commerce]。

不映射到首選承運人的商業承運人被標籤為 *[!UICONTROL Other Carrier]* 上 [!DNL Walmart]。

**先決條件**

在映射發運承運人之前，請完成以下任務：

1. 查看 [承運人方法和運輸最佳實踐](https://sellerhelp.walmart.com/s/guide?article=000009473) 為 [!DNL Walmart Marketplace]。

1. 驗證 [[!UICONTROL Shipping Carrier]](https://docs.magento.com/user-guide/shipping/carriers.html) 和 [[!UICONTROL Shipping Settings]](https://docs.magento.com/user-guide/configuration/sales/shipping-settings.html) 配置 [!DNL Commerce] 儲存以確保已針對 [!DNL Walmart Marketplace sales]。

## 映射運輸承運人

1. 從 **[!UICONTROL Listings]** 或 **[!UICONTROL Orders]** ，選擇 **[!UICONTROL Channel Settings]**。

1. 開 **[!UICONTROL Channel Settings]**&#x200B;選中 **[!UICONTROL Shipping Carriers]**。

   ![映射運輸承運人](assets/map-shipping-carriers.png)

1. 每個 [!DNL Walmart] 列出首選承運人，選擇 [!DNL Commerce] 承運人名稱（如果承運人可用）。

1. 選擇 **[!UICONTROL Save]** 按鈕。
