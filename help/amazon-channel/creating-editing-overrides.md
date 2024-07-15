---
title: 建立及編輯Amazon銷售管道覆寫
description: 使用AmazonSales Channel覆寫，將您的變更套用至單一Amazon清單或多個清單。
feature: Sales Channels, Products, Configuration
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# 建立和編輯覆寫

您可以建立及覆寫清單，或編輯或移除已套用至清單的覆寫。 覆寫為特定清單設定定義的值。

## 為單一清單建立覆寫

檢視&#x200B;_[!UICONTROL Inactive]_、_[!UICONTROL Active]_&#x200B;和&#x200B;_[!UICONTROL Ineligible]_索引標籤上的清單時，_[!UICONTROL Create Override]_&#x200B;動作可用。

1. 檢視&#x200B;_[!UICONTROL Products Listings]_頁面（_[!UICONTROL Inactive]_、_[!UICONTROL Active]_和_[!UICONTROL Ineligible]_&#x200B;索引標籤）上的清單。

1. 在&#x200B;_[!UICONTROL Action]_欄中，按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**以開啟產品清單覆寫頁面。

   ![建立Amazon清單覆寫](assets/amazon-select-create-override.png){width="220"}

1. 為確保您檢視正確的清單，請驗證&#x200B;_[!UICONTROL Listing Details]_。

1. 決定您正在建立的覆寫型別。

   您可以定義清單的單一覆寫型態或任何型態組合（「價格」、「處理時間」、「條件」、「賣方備註」）。

   - **價格** — 按一下&#x200B;**[!UICONTROL Change Listing Price]**&#x200B;並輸入您為&#x200B;**[!UICONTROL Price Override]**&#x200B;定義的價格值。
   - **處理時間** — 按一下&#x200B;**[!UICONTROL Change Handling Time]**&#x200B;並輸入&#x200B;**[!UICONTROL Handling Time Override]**&#x200B;的已定義時間值（以天為單位）。
   - **條件** — 按一下&#x200B;**[!UICONTROL Change Condition]**&#x200B;並為&#x200B;**[!UICONTROL Condition Override]**&#x200B;選擇正確的選項。
   - **賣家筆記** — 按一下&#x200B;**[!UICONTROL Change Seller Notes]**&#x200B;並輸入&#x200B;**[!UICONTROL Seller Notes Override]**&#x200B;的筆記文字。

1. 按一下&#x200B;**[!UICONTROL Save Listing Override]**。

   _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態變更為`Relist in Progress`。 此次變更將會發佈至Amazon，並包含您下次的資料同步處理作業（如您的cron設定中所設定）。 此清單也會新增至_[!UICONTROL Overrides]_&#x200B;索引標籤。

下列範例顯示定義新價格`$55`、新處理時間`1 day`、新條件`Used; Like New`以及新賣家備註文字的覆寫。

![範例Amazon清單覆寫](assets/amazon-overrides-edit.png){width="600" zoomable="yes"}

## 編輯或移除單一清單的覆寫 {#edit-override-single-listing}

在&#x200B;_[!UICONTROL Overrides]_標籤上檢視清單時，可以使用_[!UICONTROL Edit Overrides]_&#x200B;動作。

1. 檢視&#x200B;_[!UICONTROL Product Listings]_頁面上的清單（_[!UICONTROL Overrides]_&#x200B;標籤）。

1. 在&#x200B;_[!UICONTROL Action]_欄中按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**。

   _[!UICONTROL Product Listing Overrides]_頁面隨即開啟。

   ![選取Amazon清單覆寫](assets/amazon-select-edit-overrides.png){width="125"}

1. 為確保您覆寫正確的清單，請驗證&#x200B;_[!UICONTROL Listing Details]_。

1. 若要編輯您的&#x200B;_[!UICONTROL Override]_設定，請針對您要變更的型別（價格、處理時間、條件、賣家備註）定義區段。

   若要保持覆寫型別相同，請選取`No Change To <override type>` （預設值）。 此設定保留先前定義的覆寫值不變。

   - **價格** — 按一下&#x200B;**[!UICONTROL Change Listing Price]**&#x200B;並輸入您為&#x200B;**[!UICONTROL Price Override]**&#x200B;定義的價格值。
   - **處理時間** — 按一下&#x200B;**[!UICONTROL Change Handling Time]**&#x200B;並輸入&#x200B;**[!UICONTROL Handling Time Override]**&#x200B;的已定義時間值（以天為單位）。
   - **條件** — 按一下&#x200B;**[!UICONTROL Change Condition]**&#x200B;並為&#x200B;**[!UICONTROL Condition Override]**&#x200B;選擇正確的選項。
   - **賣家筆記** — 按一下&#x200B;**[!UICONTROL Change Seller Notes]**&#x200B;並輸入&#x200B;**[!UICONTROL Seller Notes Override]**&#x200B;的筆記文字。

1. 若要移除覆寫型別，針對您要移除的每個型別，按一下&#x200B;**移除**。 如果未移除，先前定義的值會保留在覆寫中。

1. 按一下&#x200B;**[!UICONTROL Save Listing Override]**。

   _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態變更為`Relist in Progress`。 此次變更將會發佈至Amazon，並包含您下次的資料同步處理作業（如您的cron設定中所設定）。 如果清單尚未列出，清單也會新增至_[!UICONTROL Overrides]_&#x200B;索引標籤。

搭配&#x200B;_建立覆寫_&#x200B;範例。 下列範例顯示對先前建立之覆寫的編輯，該編輯會定義新價格`$50`、移除「處理時間」覆寫，並保留先前的「條件」與「賣家備註」覆寫。

![正在編輯或移除覆寫](assets/amazon-overrides-edit-2.png){width="600" zoomable="yes"}
__

## 編輯或移除多個清單的覆寫 {#edit-override-multiple-listings}

_[!UICONTROL Edit Listing Overrides]_動作可在_[!UICONTROL Inactive]_、_[!UICONTROL Active]_、_[!UICONTROL Overrides]_&#x200B;和&#x200B;_[!UICONTROL Ineligible]_標籤上使用。

>[!NOTE]
>
>由於您正在修改多個清單的覆寫，因此&#x200B;_[!UICONTROL Listing Details]_區段不會像修改單一清單時一樣顯示。

1. 檢視&#x200B;_[!UICONTROL Products Listings]_頁面（_[!UICONTROL Inactive]_、_[!UICONTROL Active]_、_[!UICONTROL Overrides]_&#x200B;和&#x200B;_[!UICONTROL Ineligible]_索引標籤）上的清單。

1. 選取左欄中每個要修改清單的核取方塊。

1. 在&#x200B;_[!UICONTROL Actions]_底下，按一下&#x200B;**[!UICONTROL Edit Listing Overrides]**。

   _[!UICONTROL Product Listing Overrides]_頁面隨即開啟。

   ![選取Amazon清單覆寫](assets/amazon-actions-edit-listing-overrides.png){width="200"}

1. 若要編輯您的&#x200B;_[!UICONTROL Override]_設定，請針對您要變更的型別（價格、處理時間、條件、賣家備註）定義區段。

   若要維持覆寫不變，請選取`No Change To <override type>` （預設）。 此設定保留先前定義的覆寫值不變。

   - **價格** — 按一下&#x200B;**[!UICONTROL Change Listing Price]**&#x200B;並輸入您為&#x200B;**[!UICONTROL Price Override]**&#x200B;定義的價格值。
   - **處理時間** — 按一下&#x200B;**[!UICONTROL Change Handling Time]**&#x200B;並輸入&#x200B;**[!UICONTROL Handling Time Override]**&#x200B;的已定義時間值（以天為單位）。
   - **條件** — 按一下&#x200B;**[!UICONTROL Change Condition]**&#x200B;並為&#x200B;**[!UICONTROL Condition Override]**&#x200B;選擇正確的選項。
   - **賣家筆記** — 按一下&#x200B;**[!UICONTROL Change Seller Notes]**&#x200B;並輸入&#x200B;**[!UICONTROL Seller Notes Override]**&#x200B;的筆記文字。

1. 若要移除覆寫型別，請按一下您要移除的每個型別&#x200B;**[!UICONTROL Remove]**。 如果未移除，先前定義的值會保留在覆寫中。

1. 按一下&#x200B;**[!UICONTROL Save Listing Override]**。

   _[!UICONTROL Product Listing Overrides]_頁面關閉。 清單的狀態變更為`Relist in Progress`。 此次變更將會發佈至Amazon，並包含您下次的資料同步處理作業（如您的cron設定中所設定）。 如果清單尚未列出，清單也會新增至_[!UICONTROL Overrides]_&#x200B;索引標籤。

### 覆寫型別

| 覆寫 | 說明 |
|-------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Override] | 價格修訂會定義清單的價格。 此覆寫優先於所有自動設定，直到移除覆寫為止。<br><br>若要覆寫您的產品價格，請選擇&#x200B;**[!UICONTROL Change Listing Price]**&#x200B;並輸入&#x200B;**[!UICONTROL Price Override]**&#x200B;的新價格。 |
| [!UICONTROL Handling Time Override] | 處理時間覆寫會定義處理和出貨產品所需的時間（以天為單位）。 處理時間覆寫優先於所有自動化和預設的處理時間設定，直到覆寫被移除為止。<br><br> _[!UICONTROL Handling Time Override]_方塊中的值可能是您在[清單設定](./listing-settings.md)中定義的預設處理時間，或是您定義的覆寫處理時間。 如果您移除處理時間覆寫，清單會預設為您清單設定中定義的處理時間。<br><br>若要定義處理時間覆寫，請選擇&#x200B;**[!UICONTROL Change Handling Time]**並輸入&#x200B;**[!UICONTROL Handling Time Override]**的新處理時間（以天為單位）。 |
| [!UICONTROL Condition Override] | 若要覆寫清單條件，請選擇&#x200B;**[!UICONTROL Change Condition]**&#x200B;並從&#x200B;**條件覆寫**&#x200B;中選擇新條件。 |
| [!UICONTROL Seller Notes Override] | 對於目錄中已定義條件非`New`的產品，可以新增賣家備註，向潛在買家進一步詳細說明您的產品及其條件。 您可以為`New`條件產品輸入賣家備註覆寫，但Amazon不會顯示備註。<br><br>若要覆寫賣家備註，請選擇&#x200B;**[!UICONTROL Change Seller Notes]**&#x200B;並輸入&#x200B;**[!UICONTROL Seller Notes Override]**&#x200B;的新備註。 |
