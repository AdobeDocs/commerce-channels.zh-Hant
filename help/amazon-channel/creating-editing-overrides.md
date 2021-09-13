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

在&#x200B;_[!UICONTROL Inactive]_、_[!UICONTROL Active]_&#x200B;和&#x200B;_[!UICONTROL Ineligible]_標籤上查看清單時，_[!UICONTROL Create Override]_&#x200B;操作可用。

1. 查看&#x200B;_[!UICONTROL Products Listings]_頁（_[!UICONTROL Inactive]_、_[!UICONTROL Active]_和_[!UICONTROL Ineligible]_&#x200B;頁簽）上的清單。

1. 在&#x200B;_[!UICONTROL Action]_欄中，按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**以開啟「產品清單覆蓋」頁面。

   ![建立Amazon清單覆寫](assets/amazon-select-create-override.png)

1. 為確保查看正確的清單，請驗證&#x200B;_[!UICONTROL Listing Details]_。

1. 決定您建立的覆寫類型。

   您可以為清單定義單個改寫類型或任何類型的組合（價格、處理時間、條件、賣方附註）。

   - **價格**  — 按一 **[!UICONTROL Change Listing Price]** 下並輸入您定義的價 **[!UICONTROL Price Override]**&#x200B;格值。
   - **處理時間**  — 按一 **[!UICONTROL Change Handling Time]** 下並輸入（以天為單位）的定義時 **[!UICONTROL Handling Time Override]**&#x200B;間值。
   - **條件**  — 按一 **[!UICONTROL Change Condition]** 下並為選擇正確的選 **[!UICONTROL Condition Override]**&#x200B;項。
   - **賣家附註**  — 按一 **[!UICONTROL Change Seller Notes]** 下並輸入附註文 **[!UICONTROL Seller Notes Override]**&#x200B;字。

1. 按一下&#x200B;**[!UICONTROL Save Listing Override]**。

   _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態將更改為`Relist in Progress`。 變更將隨您的下次資料同步發佈至Amazon（如您的cron設定中所設定）。 清單也會新增至_[!UICONTROL Overrides]_&#x200B;標籤。

以下示例顯示一個覆蓋，該覆蓋定義了新價格`$55`、新處理時間`1 day`、新條件`Used; Like New`和新的賣方附註文本。

![Amazon清單覆寫範例](assets/amazon-overrides-edit.png)

## 編輯或移除單一清單的覆寫 {#edit-override-single-listing}

在&#x200B;_[!UICONTROL Overrides]_標籤上檢視清單時，可使用_[!UICONTROL Edit Overrides]_&#x200B;動作。

1. 查看&#x200B;_[!UICONTROL Product Listings]_頁（_[!UICONTROL Overrides]_&#x200B;頁簽）上的清單。

1. 在&#x200B;_[!UICONTROL Action]_欄中，按一下「**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**」。

   _[!UICONTROL Product Listing Overrides]_頁面隨即開啟。

   ![選取Amazon清單覆寫](assets/amazon-select-edit-overrides.png)

1. 要確保覆蓋正確的清單，請驗證&#x200B;_[!UICONTROL Listing Details]_。

1. 要編輯&#x200B;_[!UICONTROL Override]_設定，請定義要更改的類型（價格、處理時間、條件、賣家附註）的部分。

   要保持覆蓋類型相同，請選擇`No Change To <override type>`（預設值）。 此設定會維持先前定義的覆寫值不變。

   - **價格**  — 按一 **[!UICONTROL Change Listing Price]** 下並輸入您定義的價 **[!UICONTROL Price Override]**&#x200B;格值。
   - **處理時間**  — 按一 **[!UICONTROL Change Handling Time]** 下並輸入（以天為單位）的定義時 **[!UICONTROL Handling Time Override]**&#x200B;間值。
   - **條件**  — 按一 **[!UICONTROL Change Condition]** 下並為選擇正確的選 **[!UICONTROL Condition Override]**&#x200B;項。
   - **賣家附註**  — 按一 **[!UICONTROL Change Seller Notes]** 下並輸入附註文 **[!UICONTROL Seller Notes Override]**&#x200B;字。

1. 要刪除覆蓋類型，請按一下&#x200B;**刪除**&#x200B;以刪除要刪除的每種類型。 如果未移除，先前定義的值會保留在覆寫中。

1. 按一下&#x200B;**[!UICONTROL Save Listing Override]**。

   _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態將更改為`Relist in Progress`。 變更將隨您的下次資料同步發佈至Amazon（如您的cron設定中所設定）。 如果尚未列出，清單也會新增至_[!UICONTROL Overrides]_&#x200B;標籤。

根據&#x200B;_建立覆寫_&#x200B;範例。 下面的示例顯示對先前建立的覆蓋的編輯，該覆蓋定義了新價格`$50`、刪除「處理時間」覆蓋，並保留先前的「條件」和「賣方附註」覆蓋。

![編輯或移除覆寫](assets/amazon-overrides-edit-2.png)
__

## 編輯或移除多個清單的覆寫 {#edit-override-multiple-listings}

_[!UICONTROL Edit Listing Overrides]_動作可在_[!UICONTROL Inactive]_、_[!UICONTROL Active]_、_[!UICONTROL Overrides]_&#x200B;和&#x200B;_[!UICONTROL Ineligible]_標籤上使用。

>[!NOTE]
>
>由於您正在修改多個清單的覆蓋，_[!UICONTROL Listing Details]_區段不會像修改單一清單時一樣顯示。

1. 查看&#x200B;_[!UICONTROL Products Listings]_頁（_[!UICONTROL Inactive]_、_[!UICONTROL Active]_、_[!UICONTROL Overrides]_&#x200B;和&#x200B;_[!UICONTROL Ineligible]_頁簽）上的清單。

1. 在左側欄中，選取您要修改之每個清單的核取方塊。

1. 在&#x200B;_[!UICONTROL Actions]_下，按一下&#x200B;**[!UICONTROL Edit Listing Overrides]**。

   _[!UICONTROL Product Listing Overrides]_頁面隨即開啟。

   ![選取Amazon清單覆寫](assets/amazon-actions-edit-listing-overrides.png)

1. 要編輯&#x200B;_[!UICONTROL Override]_設定，請定義要更改的類型（價格、處理時間、條件、賣家附註）的部分。

   若要保持覆蓋相同，請選擇`No Change To <override type>`（預設值）。 此設定會維持先前定義的覆寫值不變。

   - **價格**  — 按一 **[!UICONTROL Change Listing Price]** 下並輸入您定義的價 **[!UICONTROL Price Override]**&#x200B;格值。
   - **處理時間**  — 按一 **[!UICONTROL Change Handling Time]** 下並輸入（以天為單位）的定義時 **[!UICONTROL Handling Time Override]**&#x200B;間值。
   - **條件**  — 按一 **[!UICONTROL Change Condition]** 下並為選擇正確的選 **[!UICONTROL Condition Override]**&#x200B;項。
   - **賣家附註**  — 按一 **[!UICONTROL Change Seller Notes]** 下並輸入附註文 **[!UICONTROL Seller Notes Override]**&#x200B;字。

1. 要刪除覆蓋類型，請按一下&#x200B;**[!UICONTROL Remove]**&#x200B;以獲取要刪除的每種類型。 如果未移除，先前定義的值會保留在覆寫中。

1. 按一下&#x200B;**[!UICONTROL Save Listing Override]**。

   _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態將更改為`Relist in Progress`。 變更將隨您的下次資料同步發佈至Amazon（如您的cron設定中所設定）。 如果尚未列出，清單也會新增至_[!UICONTROL Overrides]_&#x200B;標籤。

### 覆蓋類型

| 覆寫 | 說明 |
|--- |--- |
| [!UICONTROL Price Override] | 價格覆蓋定義了清單的價格。 此覆寫優先於所有自動設定，直到移除覆寫為止。<br><br>要改寫產品的價格，請選 **[!UICONTROL Change Listing Price]** 擇並輸入新的 **[!UICONTROL Price Override]**&#x200B;價格。 |
| [!UICONTROL Handling Time Override] | 處理時間覆蓋定義了處理和發運產品所花費的時間（以天為單位）。 處理時間覆蓋優先於所有自動和預設的處理時間設定，直到移除覆蓋為止。<br><br>該框中存在的值是您 _[!UICONTROL Handling Time Override]_在清單設定中定義的預設處理時間， [或](./listing-settings.md) 您定義的覆蓋處理時間。如果刪除處理時間覆蓋，則清單預設為清單設定中定義的處理時間。<br><br>要定義處理時間改寫，請選&#x200B;**[!UICONTROL Change Handling Time]**擇並輸入新的處理時間(以天為單&#x200B;**[!UICONTROL Handling Time Override]**位)。 |
| [!UICONTROL Condition Override] | 要覆蓋清單條件，請選擇&#x200B;**[!UICONTROL Change Condition]**&#x200B;並從&#x200B;**條件覆蓋**&#x200B;中選擇新條件。 |
| [!UICONTROL Seller Notes Override] | 對於目錄中以`New`以外的條件定義的產品，可以添加銷售者注釋，以進一步詳細說明您的產品及其條件給潛在購買者。 您可以為`New`條件產品輸入銷售者附註改寫，但Amazon不會顯示附註。<br><br>要改寫「賣方附註」，請 **[!UICONTROL Change Seller Notes]** 選擇並輸入新的附註 **[!UICONTROL Seller Notes Override]**。 |
