---
title: 管理清單
description: 管理銷售渠道清單 [!DNL Commerce] 與Channel Manager一起儲存，用於Adobe Commerce和Magento Open Source。
exl-id: 70999552-9ba7-4b10-a8ee-ee99bc4fe837
source-git-commit: 41a6afec60edbb23492627bd8e80632d3c952caf
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 0%

---

# 管理清單

管理連接渠道的產品清單 [!UICONTROL Listings] 在渠道商店視圖中。

使用 *[!UICONTROL Listings]* 工作區以管理 [!DNL Commerce] 產品在沃爾瑪市場上出售。 單個清單的「狀態」(Status)指明產品在 [!DNL Channel Manager] 工作流，以便您可以確定後續步驟並解決任何錯誤。

![連接的銷售渠道的清單頁面](assets/products-submit-for-matching.png)

## 查看清單

1. 從管理員，轉到 [!UICONTROL **營銷** >通道> **渠道管理器**]。

1. 從「渠道商店」清單中，選擇商店條目行中的鉛筆表徵圖以開啟商店視圖。

1. 選擇 [!UICONTROL **清單**]。

## 將Commerce產品添加到Channel Manager

完成以下任務，為Walmart Marketplace渠道建立產品分類：

* [將產品從您的Commerce產品目錄添加到Channel Manager](add-products-to-connected-channel.md)

* [配置產品匹配](map-product-attributes-for-matching.md#configure-product-attribute-settings)

## 向沃爾瑪發佈產品

您可以使用產品匹配或通過手動上載新產品的產品清單在沃爾瑪市場上建立產品優惠。 有關說明，請參見 [將清單發佈到沃爾瑪市場](publish-listings-to-marketplace.md) 如以下主題中所述：

* **[在沃爾瑪上匹配產品](publish-listings-to-marketplace.md)** — 將產品清單從您的渠道發佈到 [!DNL Walmart Marketplace] 通過更新銷售相同產品的現有清單。 匹配條件由 [屬性映射配置](map-product-attributes-for-matching.md) 你的頻道。

* **[手動上載新清單](publish-listings-to-marketplace.md#upload-new-product-listings)-** — 對於與沃爾瑪市場上現有清單不匹配的產品，請使用沃爾瑪產品類別Excel模板批量上傳產品清單。

## 列出控制項和列說明

下表介紹了可用於 [!UICONTROL Listings]。

**控制項[!UICONTROL Listings]**

| **控制項** | **說明** |
|----------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Refresh products] | 使用最新清單和狀態更新顯示。 |
| [!UICONTROL Add Products] | 開啟 [!UICONTROL Admin Product Catalog] 頁面選擇要添加到 [!DNL Walmart Marketplace] 或更新產品屬性以滿足沃爾瑪市場清單要求。 |
| [!UICONTROL Match products on Walmart] | 在選擇一個或多個處於「草稿」狀態的產品後，選擇「在沃爾瑪上匹配產品」以檢查是否可以添加到現有產品中的產品優惠 [!DNL Walmart Marketplace] 清單。 |


**列說明**

| **欄位** | **說明** |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product name] | 來自的產品名稱 [!DNL Commerce] 儲存目錄。 |
| [!UICONTROL SKU (Unique ID)] | 用於匹配市場上產品的映射屬性。 此欄位名稱因映射的屬性配置而異 [!DNL Channel Manager] 清單。 在此情況下，產品匹配操作使用 [!DNL Commerce] 要查找的目錄 [!DNL Walmart Marketplace]  列出的SKU值與 [!DNL Commerce] 產品屬性。 |
| [!UICONTROL  Quantity] | 在Adobe Commerce或Magento Open Source的庫存量。 |
| [!UICONTROL Price] | 來自 [!DNL Commerce] 儲存目錄。 目錄價格更新將同步到Channel Manager，然後發送到 [!DNL Walmart Marketplace]  讓列出的項目顯示當前價格。 |
| [!UICONTROL Status] | 指示中的當前訂單狀態 [!DNL Commerce] 訂單工作流。 成功將產品添加到時的狀態更新 [!DNL Channel Manager] 和市場上的產品匹配。 如果操作失敗，清單將顯示錯誤狀態。 修復錯誤後， [!DNL Channel Manager] 重試該操作並更新狀態。 |


### 關於清單狀態

在「清單」工作區中，「狀態」標籤顯示產品在 [!DNL Channel Manager] 工作流，以便您可以確定後續步驟並解決錯誤。 清單可以具有以下狀態標籤：

* **[!UICONTROL Draft]** — 標識尚未 [已提交 [!DNL Walmart] 匹配](publish-listings-to-marketplace.md#match-products)。

* **[!UICONTROL Processing]** — 標識在上提交供匹配的產品 [!DNL Walmart Marketplace]。 產品仍在 *處理* 狀態直到 [!DNL Walmart] 返回HTTP狀態消息，該消息指示匹配是否成功或是否出現錯誤。 要完成匹配操作，最多需要30分鐘 [!DNL Walmart Marketplace]。

* **[!UICONTROL Match]** — 標識成功匹配的產品 [!DNL Walmart]。

   當產品屬性值 — 例如UPC代碼與現有產品中的UPC值匹配時，會出現匹配[!DNL Walmart Marketplace] 清單。 當產品匹配時，商務產品優惠將添加到沃爾瑪現有的清單中。

   檢查 [[!UICONTROL Walmart Marketplace Seller Account Items]](https://seller.walmart.com/items-and-inventory/manage-items) 控制面板：複查更新的產品清單並驗證產品詳細資訊、價格和庫存數量。


* **[!UICONTROL Error]** — 標識與現有產品不匹配的產品 [!DNL Walmart Marketplace] 清單。 通過懸停在 *錯誤* 狀態標籤。

   解決錯誤後，請重新提交產品以進行匹配。 請參閱 [排除產品匹配錯誤](https://docs.google.com/document/d/1bEbCyVLXJQQsbZvEwetJvZKWQJOKoiw5Ia1uB4Bs4uo/edit#heading=h.sz6eji8z9vzy)。

* **[!UICONTROL Error - Match in Stage]** — 標識上匹配的產品 [!DNL Walmart] 直到 [!DNL Walmart Marketplace] 商店是即時的。 當 [!DNL Walmart Marketplace] 商店就要開始了。
