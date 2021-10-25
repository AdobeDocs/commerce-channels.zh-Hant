---
title: 建立和編輯覆蓋
description: 使用AmazonSales Channel覆寫將變更套用至單一Amazon清單或多個清單。
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# 建立和編輯覆蓋

您可以建立和覆蓋清單，或編輯或移除已套用至清單的覆蓋。 覆蓋為特定清單設定定義值。

## 為單一清單建立覆蓋

此 _[!UICONTROL Create Override]_在上檢視清單時，可使用動作_[!UICONTROL Inactive]_, _[!UICONTROL Active]_，和_[!UICONTROL Ineligible]_ 標籤。

1. 檢視 _[!UICONTROL Products Listings]_頁面(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_，和_[!UICONTROL Ineligible]_ 標籤)。

1. 在 _[!UICONTROL Action]_欄，按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**開啟「產品清單覆蓋」頁。

   ![建立Amazon清單覆寫](assets/amazon-select-create-override.png)

1. 若要確保您檢視的清單正確無誤，請確認 _[!UICONTROL Listing Details]_.

1. 決定您建立的覆寫類型。

   您可以為清單定義單個改寫類型或任何類型的組合（價格、處理時間、條件、賣方附註）。

   - **價格**  — 按一下 **[!UICONTROL Change Listing Price]** 並為 **[!UICONTROL Price Override]**.
   - **處理時間**  — 按一下 **[!UICONTROL Change Handling Time]** 並輸入以天為單位的定義時間值 **[!UICONTROL Handling Time Override]**.
   - **條件**  — 按一下 **[!UICONTROL Change Condition]** 並為 **[!UICONTROL Condition Override]**.
   - **賣家筆記**  — 按一下 **[!UICONTROL Change Seller Notes]** 並輸入附註文字 **[!UICONTROL Seller Notes Override]**.

1. 按一下 **[!UICONTROL Save Listing Override]**.

   此 _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態變更為 `Relist in Progress`. 變更將隨您的下次資料同步發佈至Amazon（如您的cron設定中所設定）。 清單也會新增至_[!UICONTROL Overrides]_ 標籤。

下列範例顯示一個覆寫，其定義 `$55`，新的處理時間 `1 day`，是 `Used; Like New`，以及新的「賣家注釋」文本。

![Amazon清單覆寫範例](assets/amazon-overrides-edit.png)

## 編輯或移除單一清單的覆寫 {#edit-override-single-listing}

此 _[!UICONTROL Edit Overrides]_在上檢視清單時，可使用動作_[!UICONTROL Overrides]_ 標籤。

1. 檢視 _[!UICONTROL Product Listings]_頁面(_[!UICONTROL Overrides]_ 標籤)。

1. 在 _[!UICONTROL Action]_欄，按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**.

   此 _[!UICONTROL Product Listing Overrides]_頁面開啟。

   ![選取Amazon清單覆寫](assets/amazon-select-edit-overrides.png)

1. 若要確保您覆寫正確的清單，請確認 _[!UICONTROL Listing Details]_.

1. 若要編輯 _[!UICONTROL Override]_設定，為要更改的類型（價格、處理時間、條件、賣方附註）定義部分。

   要使覆蓋類型保持相同，請選擇 `No Change To <override type>` （預設）。 此設定會維持先前定義的覆寫值不變。

   - **價格**  — 按一下 **[!UICONTROL Change Listing Price]** 並為 **[!UICONTROL Price Override]**.
   - **處理時間**  — 按一下 **[!UICONTROL Change Handling Time]** 並輸入以天為單位的定義時間值 **[!UICONTROL Handling Time Override]**.
   - **條件**  — 按一下 **[!UICONTROL Change Condition]** 並為 **[!UICONTROL Condition Override]**.
   - **賣家筆記**  — 按一下 **[!UICONTROL Change Seller Notes]** 並輸入附註文字 **[!UICONTROL Seller Notes Override]**.

1. 若要移除覆寫類型，請按一下 **移除** 針對您要移除的每種類型。 如果未移除，先前定義的值會保留在覆寫中。

1. 按一下 **[!UICONTROL Save Listing Override]**.

   此 _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態變更為 `Relist in Progress`. 變更將隨您的下次資料同步發佈至Amazon（如您的cron設定中所設定）。 如果尚未列出，清單也會新增至_[!UICONTROL Overrides]_ 標籤。

搭上 _建立覆蓋_ 範例。 下列範例顯示對先前建立之覆寫的編輯，該覆寫會定義 `$50`，刪除「處理時間」覆蓋，並保留以前的「條件」和「賣方附註」覆蓋。

![編輯或移除覆寫](assets/amazon-overrides-edit-2.png)
__

## 編輯或移除多個清單的覆寫 {#edit-override-multiple-listings}

此 _[!UICONTROL Edit Listing Overrides]_動作可在_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_，和 _[!UICONTROL Ineligible]_頁簽。

>[!NOTE]
>
>由於您正在修改多個清單的覆寫，因此 _[!UICONTROL Listing Details]_修改單一清單時，區段不會如此顯示。

1. 查看 _[!UICONTROL Products Listings]_頁面(_[!UICONTROL Inactive]_, _[!UICONTROL Active]_,_[!UICONTROL Overrides]_，和 _[!UICONTROL Ineligible]_標籤)。

1. 在左側欄中，選取您要修改之每個清單的核取方塊。

1. 在 _[!UICONTROL Actions]_，按一下&#x200B;**[!UICONTROL Edit Listing Overrides]**.

   此 _[!UICONTROL Product Listing Overrides]_頁面開啟。

   ![選取Amazon清單覆寫](assets/amazon-actions-edit-listing-overrides.png)

1. 若要編輯 _[!UICONTROL Override]_設定，為要更改的類型（價格、處理時間、條件、賣方附註）定義部分。

   若要保留相同的覆寫，請選取 `No Change To <override type>` （預設）。 此設定會維持先前定義的覆寫值不變。

   - **價格**  — 按一下 **[!UICONTROL Change Listing Price]** 並為 **[!UICONTROL Price Override]**.
   - **處理時間**  — 按一下 **[!UICONTROL Change Handling Time]** 並輸入以天為單位的定義時間值 **[!UICONTROL Handling Time Override]**.
   - **條件**  — 按一下 **[!UICONTROL Change Condition]** 並為 **[!UICONTROL Condition Override]**.
   - **賣家筆記**  — 按一下 **[!UICONTROL Change Seller Notes]** 並輸入附註文字 **[!UICONTROL Seller Notes Override]**.

1. 若要移除覆寫類型，請按一下 **[!UICONTROL Remove]** 針對您要移除的每種類型。 如果未移除，先前定義的值會保留在覆寫中。

1. 按一下 **[!UICONTROL Save Listing Override]**.

   此 _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態會變更為 `Relist in Progress`. 變更將隨您的下次資料同步發佈至Amazon（如您的cron設定中所設定）。 如果尚未列出，清單也會新增至_[!UICONTROL Overrides]_ 標籤。

### 覆蓋類型

| 覆寫 | 說明 |
|--- |--- |
| [!UICONTROL Price Override] | 價格覆蓋定義了清單的價格。 此覆寫優先於所有自動設定，直到移除覆寫為止。<br><br>要改寫產品的價格，請選擇 **[!UICONTROL Change Listing Price]** 並輸入 **[!UICONTROL Price Override]**. |
| [!UICONTROL Handling Time Override] | 處理時間覆蓋定義了處理和發運產品所花費的時間（以天為單位）。 處理時間覆蓋優先於所有自動和預設的處理時間設定，直到移除覆蓋為止。<br><br>存在於 _[!UICONTROL Handling Time Override]_框中定義的預設處理時間 [清單設定](./listing-settings.md) 或您定義的覆寫處理時間。 如果刪除處理時間覆蓋，則清單預設為清單設定中定義的處理時間。<br><br>要定義處理時間覆蓋，請選擇&#x200B;**[!UICONTROL Change Handling Time]**並輸入新的處理時間（以天為單位）**[!UICONTROL Handling Time Override]**. |
| [!UICONTROL Condition Override] | 要覆蓋清單條件，請選擇 **[!UICONTROL Change Condition]** 並選擇新條件 **條件覆寫**. |
| [!UICONTROL Seller Notes Override] | 針對目錄中以 `New`，您可以新增銷售者附註，以進一步詳細說明您的產品及其條件給潛在買家。 您可以為 `New` 條件產品，但Amazon不會顯示附註。<br><br>要改寫「賣方附註」，請選擇 **[!UICONTROL Change Seller Notes]** 並輸入新備注 **[!UICONTROL Seller Notes Override]**. |
