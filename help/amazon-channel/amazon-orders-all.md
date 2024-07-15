---
title: 檢視Amazon訂單
description: 在Adobe Commerce或Magento Open Source管理員中檢視您的Amazon Marketplace訂單。
feature: Sales Channels, Orders
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 檢視Amazon訂單

檢視您Amazon訂單的方式有兩種： _[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_。

這兩個選項都會顯示從Amazon收到的基本訂單資訊，包括：

- 購買日期
- 訂單編號
- 狀態
- 購買者姓名
- 全部總計
- 訂購備註

_[!UICONTROL All Orders]_檢視新增訂單搜尋的篩選選項。

>[!NOTE]
>
>除了&#x200B;_[!UICONTROL Order Notes]_資料行之外，_[!UICONTROL Amazon orders]_&#x200B;資料表已填入從Amazon收到的訂單資訊。 _訂單備註_&#x200B;資料行由[!DNL Commerce]更新，作為訂單處理。

## 最近的訂單

您可以在[商店儀表板](./amazon-store-dashboard.md)的&#x200B;_[!UICONTROL Recent Orders]_區段中檢視您最近的訂單。

![最近的訂單](assets/amazon-recent-orders-imported.png){width="600" zoomable="yes"}

### 檢視最近的Amazon訂單

1. 按一下商店資訊卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在&#x200B;_[!UICONTROL Recent Orders]_區段中檢視您的訂單。

1. 若要檢視訂單詳細資料，請按一下&#x200B;_[!UICONTROL Order Number]_欄中的Amazon訂單編號。

   訂單的&#x200B;_[!UICONTROL Amazon Order Details]_頁面隨即開啟。

## 檢視所有訂單

您可以在&#x200B;_[!UICONTROL Amazon orders]_頁面上檢視您的所有Amazon訂單（也稱為_[!UICONTROL All Orders]_&#x200B;檢視）。 Amazon訂單表格類似於商店儀表板的&#x200B;_[!UICONTROL Recent Orders]_區段，但可讓您檢視所有Amazon訂單，並使用下列篩選選項來縮小訂單清單：

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon訂單](assets/amazon-orders-list-all.png){width="600" zoomable="yes"}

### 檢視所有Amazon訂單

1. 按一下商店資訊卡上的&#x200B;**[!UICONTROL View Store]**。

1. 按一下&#x200B;_[!UICONTROL Recent Orders]_區段中的&#x200B;**[!UICONTROL All Orders]**。

1. 若要縮小清單或搜尋特定訂單編號，請完成&#x200B;**[!UICONTROL Filter by]**&#x200B;引數，然後按一下&#x200B;**[!UICONTROL Apply filters]**。

1. 若要檢視訂單詳細資料，請按一下&#x200B;_[!UICONTROL Order Number]_欄中的Amazon訂單編號。

   訂單的&#x200B;_[!UICONTROL Amazon Order Details]_頁面隨即開啟。

## 使用篩選器

您可以將篩選器套用至&#x200B;_[!UICONTROL Filter by]_區段中的訂單清單。 進行選取並按一下&#x200B;**[!UICONTROL Apply filters]**。 您套用的篩選器會顯示在訂單格線上方。

![檢視Amazon訂單的篩選器](assets/amazon-orders-filter-view.png){width="600" zoomable="yes"}

### 變更套用的篩選器

- 您可以在&#x200B;_[!UICONTROL Filter by]_區段中新增或變更您的篩選器。 按一下&#x200B;**[!UICONTROL Apply filters]**以更新訂單清單，以及出現在訂單格線上方的篩選選項。

- 您可以按一下篩選器的「`x`」，一次移除一個篩選器，或按一下「**[!UICONTROL Clear all filters]**」，一次移除所有篩選器。 移除篩選器會更新訂單清單，以及出現在訂單格線上方的篩選器選項。

- 如果您的訂單清單很長，您可以使用格線下方的分頁控制項來檢視更多訂單。

>[!TIP]
>
>有關訂單檢視的一些提示：
>
>- 如果您有多個Amazon商店整合，則可能需要在商店檢視之間切換時重新整理頁面檢視，才能更新目前商店的訂單清單和分頁檢視。
>- 依欄排序時，排序僅適用於目前的清單檢視。 篩選清單，然後排序您檢視的頁面是最佳做法。
>- 根據檢視視窗的寬度，您可能會在欄中看到重疊文字。 若要展開要繞排文字的欄，請加寬視窗檢視。
>- 依&#x200B;_[!UICONTROL Total]_篩選時，請依整數篩選。 輸入小數點可能會造成結果錯誤。

### 預設欄

| 欄 | 說明 |
|----------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Filter by] | 僅適用於&#x200B;_[!UICONTROL All Orders]_檢視。<br>根據以下條件縮小訂單清單：<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | 從Amazon收到的購買日期。 |
| [!UICONTROL Order Number] | Amazon產生和接收的訂單編號。 若要檢視Amazon訂單詳細資訊畫面，請按一下連結。 |
| [!UICONTROL Status] | Amazon收到的訂單狀態。 選項： `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | 從Amazon收到的下訂單者名稱。 |
| [!UICONTROL Grand Total] | 從Amazon收到的訂單總貨幣值。 |
| [!UICONTROL Order Notes] | 訂單在[!DNL Commerce]中處理時記錄的最近動作。 資訊包括但不限於訂單匯入錯誤和訂單處理更新。<br>**附註**：此欄位已由[!DNL Commerce]更新為訂單處理。 |
