---
title: 檢視Amazon訂單
description: 在Adobe Commerce或Magento Open Source管理員中檢視您的Amazon Marketplace訂單。
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 檢視Amazon訂單

有兩種方式可檢視您的Amazon訂單： _[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_.

兩個選項都會顯示從Amazon收到的基本訂單資訊，包括：

- 購買日期
- 訂單編號
- 狀態
- 購買者名稱
- 總計
- 訂單附註

_[!UICONTROL All Orders]_「視圖」為訂單搜索添加篩選選項。

>[!NOTE]
>
>除了 _[!UICONTROL Order Notes]_欄、_[!UICONTROL Amazon orders]_ 表格會填入從Amazon收到的訂單資訊。 此 _訂單附註_ 欄更新者 [!DNL Commerce] 訂單處理。

## 最近訂購

您可以在 _[!UICONTROL Recent Orders]_區段 [儲存儀表板](./amazon-store-dashboard.md).

![最近訂購](assets/amazon-recent-orders-imported.png)

### 檢視最近的Amazon訂單

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在 _[!UICONTROL Recent Orders]_區段。

1. 若要檢視訂單詳細資料，請按一下 _[!UICONTROL Order Number]_欄。

   此 _[!UICONTROL Amazon Order Details]_頁面。

## 查看所有訂單

您可以在 _[!UICONTROL Amazon orders]_頁面(亦稱為_[!UICONTROL All Orders]_ 檢視)。 Amazon Orders表格類似於 _[!UICONTROL Recent Orders]_區段，但可讓您檢視所有Amazon訂單，並透過下列篩選選項縮小訂單清單的範圍：

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon訂購](assets/amazon-orders-list-all.png)

### 檢視所有Amazon訂單

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 按一下 **[!UICONTROL All Orders]** 在 _[!UICONTROL Recent Orders]_區段。

1. 要縮小清單或搜索特定訂單編號，請完成 **[!UICONTROL Filter by]** 參數，按一下 **[!UICONTROL Apply filters]**.

1. 若要檢視訂單詳細資料，請按一下 _[!UICONTROL Order Number]_欄。

   此 _[!UICONTROL Amazon Order Details]_頁面。

## 使用篩選

您可以在 _[!UICONTROL Filter by]_區段。 進行選取，然後按一下&#x200B;**[!UICONTROL Apply filters]**. 您所套用的篩選器會出現在訂單格線上方。

![檢視Amazon訂單的篩選器](assets/amazon-orders-filter-view.png)

### 變更套用的篩選

- 您可以在 _[!UICONTROL Filter by]_區段。 按一下&#x200B;**[!UICONTROL Apply filters]**以更新順序網格上方顯示的順序清單和篩選選項。

- 您可以按一下 `x` 按一下 **[!UICONTROL Clear all filters]**. 移除篩選器會更新順序清單，以及顯示在順序格線上方的篩選選項。

- 如果訂單清單很長，您可以使用格線下方的分頁控制項來檢視更多訂單。

>[!TIP]
>
>訂單檢視的幾項秘訣：
>
>- 如果您有多個Amazon商店整合，則在商店檢視之間切換時，可能需要重新整理頁面檢視，以更新目前商店的訂單清單和分頁檢視。
>- 依欄排序時，排序僅套用至目前的清單檢視。 篩選清單然後排序您檢視的頁面是最佳作法。
>- 根據視圖窗口的寬度，您可能會在列中看到重疊的文本。 若要展開要繞排的文字欄，請拓寬視窗檢視。
>- 篩選依據時 _[!UICONTROL Total]_，按整數篩選。 輸入小數量可能會導致結果中出現錯誤。


### 預設列

| 欄 | 說明 |
|---|---|
| [!UICONTROL Filter by] | 僅適用於 _[!UICONTROL All Orders]_檢視。<br>根據以下內容縮小訂單清單：<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | 從Amazon收到的購買日期。 |
| [!UICONTROL Order Number] | 由產生並從Amazon接收的訂單編號。 若要檢視「Amazon訂單詳細資料」畫面，請按一下連結。 |
| [!UICONTROL Status] | 訂單的狀態，如Amazon所收到。 選項： `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | 下訂單的人的姓名，如從Amazon收到的。 |
| [!UICONTROL Grand Total] | 從Amazon收到的訂單的總貨幣值。 |
| [!UICONTROL Order Notes] | 訂單處理時記錄的最新動作 [!DNL Commerce]. 資訊包括但不限於訂單匯入錯誤和訂單處理更新。<br>**附註**:此欄位已更新為 [!DNL Commerce] 訂單處理。 |
