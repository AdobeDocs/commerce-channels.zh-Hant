---
title: 建立別名Amazon賣家SKU
description: 您可以使用別名Amazon賣家SKU，從您的商務目錄產品建立多地區Amazon清單。
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# 建立別名Amazon賣家SKU

安 [!DNL Alias Amazon Seller SKU] 用於從您的 [!DNL Commerce] 目錄。 如果您是經驗豐富的Amazon賣家，您可能熟悉 [Amazon全球SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target=&quot;_blank&quot;}和庫存和運送專用於Marketplace的SKU。 根據Amazon銷售管道的類似原則，Amazon銷售商SKU會控制多地區層級的產品清單資訊，以及 [!DNL Alias Amazon Seller SKU] 可用來控制特定地區層級的產品清單資訊。

此函式可用來執行兩個函式：

- 建立 [!DNL Alias Amazon Seller SKU] 你的 [!DNL Commerce] 編錄產品以控制特定區域的清單資訊。

   **範例**:您是美國和加拿大地區的賣家。 請記住，在設定期間，您的每個Amazon銷售管道商店只能指派一個Amazon地區。 因此，您有Amazon銷售管道商店，其中美國地區已定義，加拿大地區則已定義。 兩家商店共用 [!DNL Commerce] 目錄，列出兩個地區的資訊，包括Amazon賣家SKU和ASIN產品屬性。 因此，目錄產品的清單在兩個商店中都相同，共用定價、庫存/數量和其他產品屬性。 但是，你的加拿大庫存來自加拿大，你的美國庫存來自美國。 因此，您應分別控制每個商店的清單數量。 若要完成此類型的地區特定控制，您可以建立別名Amazon賣家SKU。

   基本上，您可以建立連結至相同目錄產品的別名Amazon賣家SKU，並可用來重新發佈該地區的相同清單。

- 建立 [!DNL Alias Amazon Seller SKU] 並匹配 [!DNL Commerce] 將產品目錄至兩個Amazon清單。

   **範例**:您有符合Amazon清單的目錄產品。 由於Amazon經常有多個清單代表相同產品，因此您會發現相同產品的另一個Amazon清單，但Amazon已指派不同的ASIN至清單。 若要提高產品可見度以納入，您需要將目錄產品與不同的ASIN配對，並為這兩個ASIN值建立清單。 若要完成此操作，您可以建立別名Amazon賣家SKU。

   基本上，您可以建立 [!DNL Alias Amazon Seller SKU] 可用來比對單一目錄產品與第二個Amazon清單，以及為新符合的ASIN建立清單。 此情境中，同一目錄產品會有兩個Amazon清單。

   建立別名Amazon賣家SKU後，您可以使用清單設定、規則和覆寫來控制該地區的清單資訊。 可針對清單按地區定義的產品屬性包括數量/庫存、完成方法、條件、產品資格和處理時間。

## 用於特定區域的用途 {#region-specific}

檢視 _[!UICONTROL Product Listings]_頁面(_[!UICONTROL Inactive]_, _作用中_, _不合格_，或 _已結束_ 標籤)。

1. 在 _[!UICONTROL Actions]_，按一下&#x200B;**[!UICONTROL Create Alias Seller SKU]**.

1. 針對 **[!UICONTROL Assign New Seller SKU]**，輸入唯一的英數字元值。

   此值必須是唯一的（不用於目錄中的任何其他產品或別名）。

1. 針對 **[!UICONTROL Assign New ASIN]**，請不要變更。

   此值會自動填入與您目錄產品相符的產品ASIN。 根據ASIN將此值變更為兩個Amazon清單，以符合您的目錄產品。

1. 切換 **[!UICONTROL Remove Existing Seller SKU]** 選項。

   - `Yes`  — 選擇刪除清單，並使用提供的新資訊建立清單。

   - `No`  — 選擇建立清單，並保持原清單不變。

1. 按一下 **[!UICONTROL Save Listing Update]**.

## 用來比對單一目錄產品與兩個Amazon清單

1. 檢視 _[!UICONTROL Product Listings]_頁面(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_，或 _[!UICONTROL Ended]_標籤)。

1. 在 _[!UICONTROL Actions]_，按一下&#x200B;**[!UICONTROL Create Alias Seller SKU]**.

1. 針對 **[!UICONTROL Assign New Seller SKU]**，輸入唯一的英數字元值。

   此值必須是唯一的（不用於目錄中的任何其他產品或別名）。

1. 針對 **[!UICONTROL Assign New ASIN]**，輸入唯一的英數字元值。

   此值會自動填入與您目錄產品相符的產品ASIN。 根據ASIN將此值變更為兩個Amazon清單，以符合您的目錄產品。

1. 切換 **[!UICONTROL Remove Existing Seller SKU]** 選項。

   - `Yes`  — 選擇刪除清單，並使用提供的新資訊建立清單。

   - `No`  — 選擇建立另一個清單，並保持原清單不變。

1. 按一下 **[!UICONTROL Save Listing Update]**.

![建立別名Amazon賣家SKU](assets/amazon-alias-sku-create.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Assign New Seller SKU] | 輸入要連結至原始Amazon賣家SKU的新且唯一的英數字元值。 此數字僅供Amazon銷售管道用來比對您的目錄產品。 您可以使用任何SKU值，但該值只能在目錄中使用一次。 |
| [!UICONTROL Assign New ASIN] | 輸入要與目錄產品匹配的清單的ASIN值。 只有在將單一目錄產品與ASIN匹配時，才修改此欄位，以獲取相同產品的另一個清單。 此值必須符合Amazon指派的ASIN，否則Amazon不會拒絕清單。 |
| [!UICONTROL Remove Existing Seller SKU] | 選項：<ul><li>**[!UICONTROL Yes]**  — 選擇刪除清單，並使用提供的新資訊建立清單。 新清單會顯示在 _[!UICONTROL Active]_，則舊清單會移至_&#x200B;已結束&#x200B;_標籤。</li><li>**[!UICONTROL No]**  — 選擇建立另一個清單，並保持原清單不變。 建立新清單後，兩個清單都會顯示在「作用中」索引標籤中。</li></ul> |
