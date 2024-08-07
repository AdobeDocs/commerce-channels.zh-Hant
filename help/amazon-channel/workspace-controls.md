---
title: Amazon sales channel - Workspace控制項
description: AmazonSales Channel提供工作區控制項，可協助您找出清單、檢視資訊，以及輕鬆套用動作。
feature: Sales Channels
exl-id: 4f76b1d0-ae58-435b-bd6d-50155a023421
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Workspace控制項

Amazon銷售管道[首頁](./amazon-sales-channel-home.md)有一些常見的工作區控制項，包括篩選器、預設檢視、欄和匯出。 並非所有頁面都具有相同的控制選項。

![AmazonSales Channel工作區控制項範例](assets/amazon-workspace-controls.png){width="600" zoomable="yes"}

## 動作

_[!UICONTROL Actions]_選擇器提供使用者可用於頁面的動作清單。 選取後，動作會套用至所有選取的專案。 若要將動作套用至特定專案，請選取每個專案第一欄中的核取方塊，並在_[!UICONTROL Actions]_&#x200B;下選擇選項。

例如，當選取器顯示在&#x200B;_[!UICONTROL Attributes]_頁面上時，會包含_[!UICONTROL Re-import Product Attribute Values]_&#x200B;動作。 選擇此動作會偵測對應的[!DNL Amazon Seller Central]帳戶，並重新整理左側欄中每個已核取之Amazon存放區專案的[!DNL Commerce]資料。

![動作功能表範例](assets/amazon-sales-channel-home-actions-option.png){width="500"}

## 篩選器

_[!UICONTROL Filters]_控制項顯示縮小表格中所顯示資料的選項。 篩選選項是根據「欄」控制項中選取的欄而定。 篩選選項只會顯示在「欄」控制項中啟用的欄。

篩選器控制項可包含用於縮小指定日期資料範圍的動態行事曆、具有預先定義選取範圍的欄的下拉式功能表，以及可能包含自訂資料的任意文字欄位。

下列範例顯示篩選訂單清單的設定，以僅顯示符合以下條件的訂單：

- 2019年2月1日與2019年2月7日之間的訂單，以及
- 採購員名為`Smith`的訂單，並且
- 狀態為`Shipped`的訂單。

當您設定好篩選選項後，請按一下&#x200B;**[!UICONTROL Apply Filters]**&#x200B;以篩選列出的資料。 按一下「取消」結束「篩選器」控制項而不套用。

![篩選器控制項範例](assets/workspace-controls-filters.png){width="600" zoomable="yes"}

在您套用篩選器至資料後，**[!UICONTROL Active Filters]**&#x200B;資訊將會顯示。 您可以按一下「![清除篩選器」圖示](assets/x-icon-clear-filters.png)來清除特定的篩選器選項，或按一下「**[!UICONTROL Clear All]**」來清除所有套用的篩選器。

![使用中的篩選器範例](assets/applied-filters-line.png){width="700"}

## 檢視

「檢視」控制項是以頁面的預設欄為基礎，因此命名為「預設檢視」。 您可以使用「欄」控制項來新增或移除可用的欄。 當您自訂欄時，可以將檢視儲存為「檢視」控制項中的自訂檢視。

在頁面顯示中新增或移除欄時：

1. 按一下&#x200B;**[!UICONTROL Default View]** > **[!UICONTROL Save View As...]**。

1. 輸入檢視的名稱。

1. 若要儲存自訂檢視，請按一下箭頭圖示。

![檢視控制項範例](assets/workspace-controls-view.png)

在此範例中，_訂單ID_&#x200B;欄新增至Column控制項中，並儲存為自訂檢視。 請注意，儲存自訂檢視名稱后，檢視名稱會從&#x200B;_預設檢視_&#x200B;變更為輸入的名稱。

您可以在&#x200B;_[!UICONTROL View]_功能表中選取想要的檢視，以在檢視之間切換。

如果您想要刪除或變更自訂檢視的名稱，請按一下鉛筆圖示。 然後您可以輸入不同的名稱，或按一下垃圾桶圖示以刪除自訂檢視。 無法刪除預設檢視。

## 欄

「欄」控制項可讓您新增或移除頁面顯示中的資料欄。 每個Amazon銷售管道頁面都具有資料欄的預設組合，但大多數頁面都有可用的其他欄。 如果沒有其他欄可用，您仍可以從顯示中移除預設欄。

下列範例顯示「欄」控制項。 核取選項對應至頁面上顯示的欄標題。

- 若要在頁面中新增資料欄，請選取核取方塊。
- 若要從頁面中移除資料欄，請勿選取核取方塊。

![資料行控制項範例](assets/workspace-controls-columns.png){width="400"}

核取方塊變更會立即顯示。 如果您進行變更並退出頁面，頁面會回到預設的欄顯示。 對於您定期進行的變更，您可以將欄變更儲存為「檢視」控制項中的自訂檢視。 然後，您就可以在「檢視」控制項中切換，而無需手動新增或移除欄。

您可以按一下「**[!UICONTROL Reset]**」將選項設定回預設設定，或按一下「**[!UICONTROL Cancel]**」結束，而不進行變更。

## 匯出

「匯出」選項可讓您將資料匯出至資料檔，而資料檔無法匯入至協力廠商軟體或個別資料庫。 匯出的資料僅限於顯示的資料。 如有需要，在使用「匯出」控制項之前，請務必新增或移除欄。

準備匯出資料時，請選擇匯出格式選項，然後按一下&#x200B;**[!UICONTROL Export]**。

- CSV — 包含純文字資料的逗號分隔值檔案
- Excel XML — 以XML為基礎的試算表資料格式（通常用於Excel使用者）

產生的資料檔案會自動儲存到您指定的資料夾以供下載。

![匯出控制](assets/workspace-controls-export.png){width="250"}
