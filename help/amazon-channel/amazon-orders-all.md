---
title: 查看Amazon訂單
description: 在Adobe Commerce或Magento Open Source管理員中查看您的Amazon市場訂單。
exl-id: d7811604-8e15-4d1a-a0e7-9fa61c61ef5d
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 查看Amazon訂單

查看您的Amazon訂單有兩種方法： _[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_。

兩個選項都向您顯示從Amazon收到的基本訂單資訊，包括：

- 採購日期
- 訂單編號
- 狀態
- 採購員姓名
- 總計
- 訂單附註

_[!UICONTROL All Orders]_「視圖」(view)為訂單搜索添加篩選選項。

>[!NOTE]
>
>除 _[!UICONTROL Order Notes]_列_[!UICONTROL Amazon orders]_ 表中填有從Amazon收到的訂單資訊。 的 _訂單附註_ 列更新者 [!DNL Commerce] 按順序排列。

## 最近訂單

您可以在 _[!UICONTROL Recent Orders]_的下界 [儲存儀表板](./amazon-store-dashboard.md)。

![最近訂單](assets/amazon-recent-orders-imported.png)

### 查看最近的Amazon訂單

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在 _[!UICONTROL Recent Orders]_的子菜單。

1. 要查看訂單詳細資訊，請按一下 _[!UICONTROL Order Number]_的雙曲餘切值。

   的 _[!UICONTROL Amazon Order Details]_的上界。

## 查看所有訂單

您可以查看您的所有Amazon訂單 _[!UICONTROL Amazon orders]_頁(也稱為_[!UICONTROL All Orders]_ )。 「Amazon訂單」表與 _[!UICONTROL Recent Orders]_的子菜單，但允許您查看所有Amazon訂單，並使用以下篩選器選項縮小訂單清單範圍：

- [!UICONTROL Purchase Date (range)]
- [!UICONTROL Order Number]
- [!UICONTROL Buyer's Name]
- [!UICONTROL Total (range)]
- [!UICONTROL Status]

![Amazon訂單](assets/amazon-orders-list-all.png)

### 查看所有Amazon訂單

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 按一下 **[!UICONTROL All Orders]** 的 _[!UICONTROL Recent Orders]_的子菜單。

1. 要縮小清單或搜索特定訂單編號，請完成 **[!UICONTROL Filter by]** 參數，按一下 **[!UICONTROL Apply filters]**。

1. 要查看訂單詳細資訊，請按一下 _[!UICONTROL Order Number]_的雙曲餘切值。

   的 _[!UICONTROL Amazon Order Details]_的上界。

## 使用篩選器

您可以將篩選器應用於訂單清單 _[!UICONTROL Filter by]_的子菜單。 進行選擇，然後按一下&#x200B;**[!UICONTROL Apply filters]**。 您應用的篩選器顯示在訂單網格的上方。

![用於查看Amazon訂單的篩選器](assets/amazon-orders-filter-view.png)

### 更改應用的篩選器

- 您可以在 _[!UICONTROL Filter by]_的子菜單。 按一下&#x200B;**[!UICONTROL Apply filters]**來更新訂單清單和出現在訂單網格上方的篩選器選項。

- 您可以通過按一下 `x` 按一下 **[!UICONTROL Clear all filters]**。 刪除篩選器會更新訂單清單以及顯示在訂單網格上方的篩選器選項。

- 如果訂單清單很長，則可以使用網格下的分頁控制項查看更多訂單。

>[!TIP]
>
>有關訂單視圖的一些提示：
>
>- 如果您有多個Amazon儲存整合，則可能需要在儲存視圖之間切換時刷新頁面視圖以更新當前儲存的訂單清單和分頁視圖。
>- 按列排序時，排序僅應用於當前清單視圖。 過濾清單，然後對您正在查看的頁面進行排序是一種最佳做法。
>- 根據視圖窗口的寬度，您可能會在列中看到重疊的文本。 要展開要換行的文本的列，請拓寬窗口視圖。
>- 篩選時 _[!UICONTROL Total]_，按整數篩選。 輸入小數量可能會導致結果出錯。


### 預設列

| 列 | 說明 |
|---|---|
| [!UICONTROL Filter by] | 僅在 _[!UICONTROL All Orders]_的子菜單。<br>根據以下各項縮小訂單清單：<ul><li>`Purchase Date (range)`</li><li>`Order Number`</li><li>`Buyer's Name`</li><li>`Total (range)`</li><li>`Status`</li></ul> |
| [!UICONTROL Purchase Date] | 購買日期，從Amazon收到。 |
| [!UICONTROL Order Number] | 由Amazon生成並從其接收的訂單號。 要查看「Amazon訂單詳細資訊」螢幕，請按一下連結。 |
| [!UICONTROL Status] | 訂單狀態，如Amazon所收。 選項： `Error` / `Pending` / `Shipped` / `Canceled` / `Completed` / `Unshipped` / `PartiallyShipped` / `PendingAvailability` |
| [!UICONTROL Buyer's Name] | 從Amazon收到的下單者的姓名。 |
| [!UICONTROL Grand Total] | 從Amazon收到的訂單的總幣種值。 |
| [!UICONTROL Order Notes] | 在中處理訂單時記錄的最新操作 [!DNL Commerce]。 資訊包括但不限於訂單導入錯誤和訂單處理更新。<br>**注釋**:此欄位由 [!DNL Commerce] 按順序排列。 |
