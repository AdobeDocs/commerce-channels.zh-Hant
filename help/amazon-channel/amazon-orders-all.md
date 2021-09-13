---
title: 檢視Amazon訂單
description: 在「Adobe商務」或「Magento Open Source管理員」中檢視您的Amazon Marketplace訂單。
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 檢視Amazon訂單

有兩種方式可檢視您的Amazon訂單：_[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_。

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
>除了&#x200B;_[!UICONTROL Order Notes]_欄，_[!UICONTROL Amazon orders]_&#x200B;表格會填入從Amazon收到的訂單資訊。 _訂單附註_&#x200B;欄會隨著訂單處理由[!DNL Commerce]更新。

## 最近訂購

您可以在[儲存控制面板](./amazon-store-dashboard.md)的&#x200B;_[!UICONTROL Recent Orders]_區段中檢視最近的訂單。

![最近訂購](assets/amazon-recent-orders-imported.png)

### 檢視最近的Amazon訂單

1. 按一下商店卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在&#x200B;_[!UICONTROL Recent Orders]_區段中檢視訂單。

1. 要查看訂單詳細資訊，請按一下&#x200B;_[!UICONTROL Order Number]_列中的Amazon訂單號。

   訂單的&#x200B;_[!UICONTROL Amazon Order Details]_頁面隨即開啟。

## 查看所有訂單

您可以在&#x200B;_[!UICONTROL Amazon orders]_頁面上檢視所有Amazon訂單（亦稱為_[!UICONTROL All Orders]_&#x200B;檢視）。 「Amazon訂單」表格類似於存放區控制面板的&#x200B;_[!UICONTROL Recent Orders]_區段，但可讓您檢視所有Amazon訂單，並透過下列篩選選項縮小訂單清單的範圍：

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon訂購](assets/amazon-orders-list-all.png)

### 查看所有Amazon訂單

1. 按一下商店卡上的&#x200B;**[!UICONTROL View Store]**。

1. 按一下&#x200B;_[!UICONTROL Recent Orders]_區段中的&#x200B;**[!UICONTROL All Orders]**。

1. 要縮小清單或搜索特定訂單編號，請完成&#x200B;**[!UICONTROL Filter by]**&#x200B;參數，然後按一下&#x200B;**[!UICONTROL Apply filters]**。

1. 要查看訂單詳細資訊，請按一下&#x200B;_[!UICONTROL Order Number]_列中的Amazon訂單號。

   訂單的&#x200B;_[!UICONTROL Amazon Order Details]_頁面隨即開啟。

## 使用篩選

您可以在&#x200B;_[!UICONTROL Filter by]_區段中將篩選器套用至訂單清單。 進行選擇，然後按一下&#x200B;**[!UICONTROL Apply filters]**。 您所套用的篩選器會出現在訂單格線上方。

![檢視Amazon訂單的篩選器](assets/amazon-orders-filter-view.png)

### 變更套用的篩選

- 您可以在&#x200B;_[!UICONTROL Filter by]_區段中新增或變更篩選器。 按一下&#x200B;**[!UICONTROL Apply filters]**以更新訂單清單以及出現在訂單網格上方的篩選選項。

- 您可以按一下篩選器的`x`一次移除一個篩選器，或按一下&#x200B;**[!UICONTROL Clear all filters]**&#x200B;一次全部移除。 移除篩選器會更新順序清單，以及顯示在順序格線上方的篩選選項。

- 如果訂單清單很長，您可以使用格線下方的分頁控制項來檢視更多訂單。

>[!TIP]
>
>訂單檢視的幾項秘訣：
>
>- 如果您有多個Amazon商店整合，則在商店檢視之間切換時，可能需要重新整理頁面檢視，以更新目前商店的訂單清單和分頁檢視。
>- 依欄排序時，排序僅套用至目前的清單檢視。 篩選清單然後排序您檢視的頁面是最佳作法。
>- 根據視圖窗口的寬度，您可能會在列中看到重疊的文本。 若要展開要繞排的文字欄，請拓寬視窗檢視。
>- 依&#x200B;_[!UICONTROL Total]_篩選時，請依整數篩選。 輸入小數量可能會導致結果中出現錯誤。


### 預設列

| 欄 | 說明 |
|---|---|
| [!UICONTROL Filter by] | 僅適用於&#x200B;_[!UICONTROL All Orders]_檢視。<br>根據以下內容縮小訂單清單：<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | 從Amazon收到的購買日期。 |
| [!UICONTROL Order Number] | 由產生並從Amazon接收的訂單編號。 若要檢視「Amazon訂單詳細資料」畫面，請按一下連結。 |
| [!UICONTROL Status] | 訂單的狀態，如Amazon所收到。 選項：`Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | 下訂單的人的姓名，如從Amazon收到的。 |
| [!UICONTROL Grand Total] | 從Amazon收到的訂單的總貨幣值。 |
| [!UICONTROL Order Notes] | 在[!DNL Commerce]中處理訂單時記錄的最新動作。 資訊包括但不限於訂單匯入錯誤和訂單處理更新。<br>**注意**:此欄位會隨著訂 [!DNL Commerce] 單處理而更新。 |
