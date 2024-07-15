---
title: 建立別名Amazon賣家SKU
description: 您可以使用別名Amazon賣家SKU，從您的Amazon目錄產品建立多區域Commerce清單。
feature: Sales Channels, Products
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 0%

---

# 建立別名Amazon賣家SKU

[!DNL Alias Amazon Seller SKU]是用來從您[!DNL Commerce]目錄中的相同產品建立Amazon清單。 如果您是有經驗的Amazon賣家，您可能熟悉[Amazon全域SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target="_blank"}以及市集特定的SKU，以便進行存貨與運送。 依照Amazon銷售管道的類似原則，Amazon賣家SKU可在多區域層級控制產品清單資訊，而[!DNL Alias Amazon Seller SKU]可用於在區域特定層級控制產品清單資訊。

此函式可用於執行兩個函式：

- 為您其中一個[!DNL Commerce]目錄產品建立[!DNL Alias Amazon Seller SKU]，以控制區域特定的清單資訊。

  **範例**：您同時是美國和加拿大地區的賣家。 請記住，在設定期間，您每個Amazon銷售管道商店只能指派一個Amazon區域。 因此，您有一個已定義美國地區的Amazon銷售管道商店，以及另一個已定義加拿大地區的商店。 兩個商店都共用您的[!DNL Commerce]目錄，以取得兩個地區的清單資訊，包括Amazon賣家SKU和ASIN產品屬性。 因此，在兩個商店中，目錄產品的清單會相同，共用定價、庫存/數量和其他產品屬性。 但是，您的加拿大商店存貨來自加拿大地點，而您的美國商店存貨來自美國地點。 因此，您應該分別控制每個商店的清單數量。 若要完成這類地區特定控制，您可以建立Amazon賣家SKU別名。

  基本上，您可以建立連結至相同目錄產品的別名Amazon賣家SKU，並可用來重新發佈該地區內的相同清單。

- 建立[!DNL Alias Amazon Seller SKU]並將您的其中一個[!DNL Commerce]目錄產品與兩個Amazon清單比對。

  **範例**：您的目錄產品符合Amazon清單。 由於Amazon經常有多個代表相同產品的清單，因此您會發現同一產品的另一個Amazon清單，但Amazon已指派其他ASIN給該清單。 若要增加產品可視性以包含，您想要將目錄產品與不同的ASIN配對，並為兩個ASIN值建立清單。 若要完成此操作，您可以建立Amazon賣家SKU別名。

  基本上，您可以建立可用來比對單一目錄產品與第二個Amazon清單的[!DNL Alias Amazon Seller SKU]，並為新比對的ASIN建立清單。 在此案例中，您會有相同目錄產品的兩個Amazon清單。

  建立Amazon賣家SKU別名後，您就可以使用清單設定、規則和覆寫來控制該區域的清單資訊。 可為清單每個區域定義的產品屬性包括數量/存貨、履行方法、條件、產品資格和處理時間。

## 用於特定區域的用途 {#region-specific}

檢視&#x200B;_[!UICONTROL Product Listings]_頁面上的清單（_[!UICONTROL Inactive]_、_使用中_、_不適用_&#x200B;或&#x200B;_已結束_&#x200B;標籤）。

1. 在&#x200B;_[!UICONTROL Actions]_底下，按一下&#x200B;**[!UICONTROL Create Alias Seller SKU]**。

1. 針對&#x200B;**[!UICONTROL Assign New Seller SKU]**，請輸入唯一的英數字元值。

   此值必須是唯一的（不適用於目錄中的任何其他產品或別名）。

1. 針對&#x200B;**[!UICONTROL Assign New ASIN]**，不做任何變更。

   此值會自動填入與目錄產品相符的產品ASIN。 變更此值會根據ASIN將您的目錄產品與兩個Amazon清單比對。

1. 視需要切換&#x200B;**[!UICONTROL Remove Existing Seller SKU]**&#x200B;選項。

   - `Yes` — 選擇刪除清單，並使用提供的新資訊建立清單。

   - `No` — 選擇建立清單，並保持舊清單不變。

1. 按一下&#x200B;**[!UICONTROL Save Listing Update]**。

## 用於將單一目錄產品與兩個Amazon清單比對

1. 檢視&#x200B;_[!UICONTROL Product Listings]_頁面（_[!UICONTROL Inactive]_、_[!UICONTROL Active]_、_[!UICONTROL Ineligible]_&#x200B;或&#x200B;_[!UICONTROL Ended]_標籤）上的清單。

1. 在&#x200B;_[!UICONTROL Actions]_底下，按一下&#x200B;**[!UICONTROL Create Alias Seller SKU]**。

1. 針對&#x200B;**[!UICONTROL Assign New Seller SKU]**，請輸入唯一的英數字元值。

   此值必須是唯一的（不適用於目錄中的任何其他產品或別名）。

1. 針對&#x200B;**[!UICONTROL Assign New ASIN]**，請輸入唯一的英數字元值。

   此值會自動填入與目錄產品相符的產品ASIN。 變更此值會根據ASIN將您的目錄產品與兩個Amazon清單比對。

1. 視需要切換&#x200B;**[!UICONTROL Remove Existing Seller SKU]**&#x200B;選項。

   - `Yes` — 選擇刪除清單，並使用提供的新資訊建立清單。

   - `No` — 選擇建立其他清單，並保持舊清單不變。

1. 按一下&#x200B;**[!UICONTROL Save Listing Update]**。

![建立別名Amazon賣家SKU](assets/amazon-alias-sku-create.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|-----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Assign New Seller SKU] | 輸入要連結至原始Amazon賣家SKU的新不重複英數字元值。 此號碼僅供Amazon銷售管道用於比對您的目錄產品。 您可以使用任何SKU值，但此值在目錄中只能使用一次。 |
| [!UICONTROL Assign New ASIN] | 輸入清單的ASIN值，以符合您的型錄產品。 只有在將單一目錄產品與ASIN比對時，才能修改此欄位，以取得相同產品的另一個清單。 此值必須與Amazon指派的ASIN相符，否則Amazon將不會拒絕此清單。 |
| [!UICONTROL Remove Existing Seller SKU] | 選項：<ul><li>**[!UICONTROL Yes]** — 選擇刪除清單，並使用提供的新資訊建立清單。 新清單會出現在&#x200B;_[!UICONTROL Active]_索引標籤中，而舊清單會移至_&#x200B;已結束&#x200B;_索引標籤。</li><li>**[!UICONTROL No]** — 選擇建立其他清單，並保持舊清單不變。 建立新清單後，兩個清單都會顯示在「作用中」標籤中。</li></ul> |
