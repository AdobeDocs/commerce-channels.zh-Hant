---
title: 建立別名Amazon賣家SKU
description: 您可以使用別名Amazon賣家SKU從您的商務目錄產品建立多區域Amazon清單。
exl-id: df3cafbf-58df-4c93-9e63-20feb6f4e7ed
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# 建立別名Amazon賣家SKU

安 [!DNL Alias Amazon Seller SKU] 用於根據您的 [!DNL Commerce] 目錄。 如果你是一位經驗豐富的Amazon賣家，您可能熟悉 [Amazon全球SKU](https://sellercentral.amazon.com/gp/help/external/help.html?itemID=201394090){target="_blank"} 和特定於市場的SKU，用於庫存和發運。 根據Amazon銷售渠道的類似原則，Amazon銷售商SKU控制多區域級產品清單資訊， [!DNL Alias Amazon Seller SKU] 可用於在特定區域級別控制產品清單資訊。

此函式可用於執行兩個函式：

- 建立 [!DNL Alias Amazon Seller SKU] 你的 [!DNL Commerce] 目錄產品以控制特定於區域的清單資訊。

   **示例**:您是美國和加拿大地區的賣家。 請記住，在設定期間，您的Amazon銷售渠道商店只能分配一個Amazon地區。 因此，您有一家Amazon銷售渠道商店，其中有一個定義的美國地區，另一家商店，其中一個定義的加拿大地區。 兩個商店共用 [!DNL Commerce] 用於列出兩個地區的資訊的目錄，包括Amazon銷售商SKU和ASIN產品屬性。 因此，目錄產品的清單在兩個商店、共用定價、庫存/數量和其他產品屬性中將是相同的。 但是，你在加拿大的存貨是從加拿大的一個地方運來的，你在美國的存貨是從美國的地方運的。 因此，您應單獨控制每個商店的清單數量。 要完成此類特定於區域的控制，您可以建立別名Amazon賣家SKU。

   實際上，您可以建立一個別名Amazon賣家SKU，該SKU連結到同一目錄產品，可用於在該區域重新發佈同一清單。

- 建立 [!DNL Alias Amazon Seller SKU] 和你 [!DNL Commerce] 將產品目錄化為兩個Amazon。

   **示例**:您有與Amazon清單匹配的目錄產品。 由於Amazon經常有多個清單代表同一產品，因此您會發現同一產品的另一個Amazon清單，但Amazon已將不同的ASIN分配給該清單。 要提高產品可視性以包括，您需要將目錄產品與不同的ASIN匹配，並為兩個ASIN值建立清單。 為了實現此目的，您可以建立別名Amazon賣家SKU。

   實際上，您可以 [!DNL Alias Amazon Seller SKU] 可用於將單個目錄產品與第二個Amazon清單匹配，並為新匹配的ASIN建立清單。 在此方案中，您將有兩個Amazon清單，用於同一目錄產品。

   建立別名Amazon賣家SKU後，您可以使用清單設定、規則和覆蓋來控制區域的清單資訊。 可以按清單區域定義的產品屬性包括數量/庫存、履行方法、條件、產品資格和處理時間。

## 用於特定區域 {#region-specific}

查看 _[!UICONTROL Product Listings]_頁(P)_[!UICONTROL Inactive]_。 _活動_。 _不合格_&#x200B;或 _結束_ )的正平方根。

1. 下 _[!UICONTROL Actions]_按一下&#x200B;**[!UICONTROL Create Alias Seller SKU]**。

1. 對於 **[!UICONTROL Assign New Seller SKU]**，輸入唯一的字母數字值。

   此值必須唯一（不用於目錄中的任何其他產品或別名）。

1. 對於 **[!UICONTROL Assign New ASIN]**，不更改。

   此值將自動填充與目錄產品匹配的產品ASIN。 更改此值將目錄產品與基於ASIN的兩個Amazon清單匹配。

1. 切換 **[!UICONTROL Remove Existing Seller SKU]** 選項。

   - `Yes`  — 選擇刪除清單並使用提供的新資訊建立清單。

   - `No`  — 選擇建立清單並保持舊清單不變。

1. 按一下 **[!UICONTROL Save Listing Update]**。

## 用於將單個目錄產品與兩個Amazon清單匹配

1. 查看 _[!UICONTROL Product Listings]_頁(P)_[!UICONTROL Inactive]_。 _[!UICONTROL Active]_。_[!UICONTROL Ineligible]_&#x200B;或 _[!UICONTROL Ended]_)。

1. 下 _[!UICONTROL Actions]_按一下&#x200B;**[!UICONTROL Create Alias Seller SKU]**。

1. 對於 **[!UICONTROL Assign New Seller SKU]**，輸入唯一的字母數字值。

   此值必須唯一（不用於目錄中的任何其他產品或別名）。

1. 對於 **[!UICONTROL Assign New ASIN]**，輸入唯一的字母數字值。

   此值將自動填充與目錄產品匹配的產品ASIN。 更改此值將目錄產品與基於ASIN的兩個Amazon清單匹配。

1. 切換 **[!UICONTROL Remove Existing Seller SKU]** 選項。

   - `Yes`  — 選擇刪除清單並使用提供的新資訊建立清單。

   - `No`  — 選擇建立另一個清單，並保持舊清單不變。

1. 按一下 **[!UICONTROL Save Listing Update]**。

![建立別名Amazon賣家SKU](assets/amazon-alias-sku-create.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Assign New Seller SKU] | 輸入要連結到原始Amazon賣家SKU的新唯一字母數字值。 此號碼僅由Amazon銷售渠道用於與目錄產品匹配。 您可以使用任何SKU值，但該值只能在目錄中使用一次。 |
| [!UICONTROL Assign New ASIN] | 輸入要與目錄產品匹配的清單的ASIN值。 僅在將單個目錄產品與ASIN匹配時，才修改此欄位，以便為同一產品的另一個清單進行匹配。 此值必須與Amazon分配的ASIN匹配，否則清單不會被Amazon拒絕。 |
| [!UICONTROL Remove Existing Seller SKU] | 選項：<ul><li>**[!UICONTROL Yes]**  — 選擇刪除清單並使用提供的新資訊建立清單。 新清單將出現在 _[!UICONTROL Active]_的子菜單。_&#x200B;結束&#x200B;_頁籤。</li><li>**[!UICONTROL No]**  — 選擇建立另一個清單，並保持舊清單不變。 建立新清單後，兩個清單都會顯示在「活動」頁籤中。</li></ul> |
