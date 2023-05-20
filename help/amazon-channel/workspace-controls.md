---
title: 工作區控制項
description: AmazonSales Channel提供工作區控制項，幫助您查找清單、查看資訊，以及輕鬆地應用操作。
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# 工作區控制項

Amazon銷售渠道 [首頁](./amazon-sales-channel-home.md) 具有一些常用工作區控制項，包括篩選器、預設視圖、列和導出。 並非所有頁面都具有相同的控制選項。

![AmazonSales Channel工作區控制示例](assets/amazon-workspace-controls.png)

## 操作

的 _[!UICONTROL Actions]_selector提供用戶可用於頁面的操作清單。 選中後，該操作將應用於所有選定項。 要將操作應用於特定項目，請選中每個項目第一列中的複選框，然後在_[!UICONTROL Actions]_。

例如，當選擇器顯示在 _[!UICONTROL Attributes]_頁面，包括_[!UICONTROL Re-import Product Attribute Values]_ 操作。 選擇此操作會ping相應 [!DNL Amazon Seller Central] 帳戶並刷新 [!DNL Commerce] 左側列中檢查的每個Amazon儲存項的資料。

![操作菜單示例](assets/amazon-sales-channel-home-actions-option.png)

## 篩選器

的 _[!UICONTROL Filters]_控制項顯示用於縮小表中顯示的資料的選項。 篩選器選項基於在「列」控制項中選擇的列。 僅顯示在「列」控制項中啟用的列的篩選器選項。

篩選器控制項可以包括動態日曆以縮小指定日期的資料範圍、具有預定義選擇的列的下拉菜單以及包含自定義資料的自由文本欄位。

以下示例顯示了用於篩選訂單清單的設定，以僅顯示符合以下條件的訂單：

- 在2/01/2019和2/07/2019之間
- 具有名為的採購員的訂單 `Smith`,
- 狀態為 `Shipped`。

設定過濾選項後，按一下 **[!UICONTROL Apply Filters]** 來篩選列出的資料。 按一下「取消」(Cancel)退出「過濾器」(Filters)控制項而不應用。

![篩選器控制項示例](assets/workspace-controls-filters.png)

在對資料應用篩選器後， **[!UICONTROL Active Filters]** 資訊。 您可以按一下 ![清除篩選器表徵圖](assets/x-icon-clear-filters.png) 表徵圖以清除特定的篩選器選項，或按一下 **[!UICONTROL Clear All]** 以清除所有應用的篩選器。

![活動篩選器示例](assets/applied-filters-line.png)

## 視圖

「視圖」(View)控制項基於頁面的預設列，因此它被命名為「預設視圖」(Default View)。 可以使用「列」(Columns)控制項添加或刪除可用列。 在自定義列時，可以在「視圖」(View)控制項中將視圖另存為自定義視圖。

在頁面顯示中添加或刪除列時：

1. 按一下 **[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**。

1. 輸入視圖名稱。

1. 要保存自定義視圖，請按一下箭頭表徵圖。

![查看控制項示例](assets/workspace-controls-view.png)

在此示例中， _訂單ID_ 列將添加到列控制項中，並另存為自定義視圖。 注意，在保存自定義視圖名稱后，視圖名稱從 _預設視圖_ 到輸入的名稱。

通過在 _[!UICONTROL View]_的子菜單。

如果要刪除或更改自定義視圖的名稱，請按一下鉛筆表徵圖。 然後，可以輸入其他名稱，或者按一下垃圾桶表徵圖以刪除自定義視圖。 無法刪除預設視圖。

## 列

「列」(Columns)控制項允許您在頁面顯示中添加或刪除資料列。 每個Amazon銷售渠道頁面都有資料列的預設組合，但大多數頁面都有其他可用列。 如果沒有其他列可用，則仍可從顯示中刪除預設列。

以下示例顯示了一個Columns控制項。 選中的選項與頁面上顯示的列標題相對應。

- 要向頁面添加資料列，請選中該複選框。
- 要從頁面中刪除資料列，請不要選中複選框。

![列控制項示例](assets/workspace-controls-columns.png)

複選框更改將立即顯示。 如果進行更改並退出頁面，頁面將返回預設列顯示。 對於您定期進行的更改，您可以在「視圖」控制項中將列更改另存為自定義視圖。 然後，您可以在「視圖」控制項中切換，而無需手動添加或刪除列。

您可以按一下 **[!UICONTROL Reset]** 將選項設定回預設設定，或者 **[!UICONTROL Cancel]** 退出。

## 導出

「導出」(Export)選項允許您將資料導出到資料檔案中，而不能導入到第三方軟體或單獨的資料庫。 導出的資料僅限於顯示的資料。 如果需要，請確保在使用「導出」控制項之前添加或刪除列。

準備好導出資料時，選擇導出格式選項，然後按一下 **[!UICONTROL Export]**。

- CSV — 包含純文字檔案資料的逗號分隔值檔案
- Excel XML — 基於XML的電子錶格資料格式（通常用於Excel用戶）

生成的資料檔案會自動保存到指定的資料夾進行下載。

![導出控制](assets/workspace-controls-export.png)
