---
title: 建立和編輯覆蓋
description: 使用AmazonSales Channel替代將您的更改應用於單個Amazon清單或多個清單。
exl-id: 3a254883-b88c-4c94-b4d5-8d7754b9afd2
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# 建立和編輯覆蓋

您可以建立和覆蓋清單，或編輯或刪除已應用於清單的覆蓋。 覆蓋為特定清單設定定義的值。

## 為單個清單建立覆蓋

的 _[!UICONTROL Create Override]_在查看清單時，操作可用_[!UICONTROL Inactive]_。 _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ 頁籤。

1. 查看清單 _[!UICONTROL Products Listings]_頁(P)_[!UICONTROL Inactive]_。 _[!UICONTROL Active]_,_[!UICONTROL Ineligible]_ )的正平方根。

1. 在 _[!UICONTROL Action]_列，按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Create Override]**開啟「產品清單覆蓋」頁。

   ![建立Amazon清單覆蓋](assets/amazon-select-create-override.png)

1. 要確保查看正確的清單，請驗證 _[!UICONTROL Listing Details]_。

1. 確定要建立的覆蓋類型。

   您可以為清單定義單個改寫類型或任何類型組合（價格、處理時間、條件、賣家附註）。

   - **價格**  — 按一下 **[!UICONTROL Change Listing Price]** 並輸入您的定價值 **[!UICONTROL Price Override]**。
   - **處理時間**  — 按一下 **[!UICONTROL Change Handling Time]** 並輸入定義的時間值（以天為單位） **[!UICONTROL Handling Time Override]**。
   - **條件**  — 按一下 **[!UICONTROL Change Condition]** 並為 **[!UICONTROL Condition Override]**。
   - **賣方便箋**  — 按一下 **[!UICONTROL Change Seller Notes]** 並輸入您的備注文本 **[!UICONTROL Seller Notes Override]**。

1. 按一下 **[!UICONTROL Save Listing Override]**。

   的 _[!UICONTROL Product Listing Overrides]_頁。 清單的狀態更改為 `Relist in Progress`。 此更改將隨您的下一次資料同步（如您的cron設定中配置）發佈到Amazon。 此清單也添加到_[!UICONTROL Overrides]_ 頁籤。

以下示例顯示定義新價格的替代 `$55`，新的處理時間 `1 day`, `Used; Like New`和新的賣家便箋文本。

![示例Amazon清單覆蓋](assets/amazon-overrides-edit.png)

## 編輯或刪除單個清單的覆蓋 {#edit-override-single-listing}

的 _[!UICONTROL Edit Overrides]_在查看清單時，操作可用_[!UICONTROL Overrides]_ 頁籤。

1. 查看 _[!UICONTROL Product Listings]_頁(P)_[!UICONTROL Overrides]_ )的正平方根。

1. 在 _[!UICONTROL Action]_列，按一下&#x200B;**[!UICONTROL Select]**>**[!UICONTROL Edit Overrides]**。

   的 _[!UICONTROL Product Listing Overrides]_的上界。

   ![選擇Amazon清單覆蓋](assets/amazon-select-edit-overrides.png)

1. 要確保覆蓋正確的清單，請驗證 _[!UICONTROL Listing Details]_。

1. 編輯 _[!UICONTROL Override]_設定，定義要更改的類型的節（價格、處理時間、條件、賣方附註）。

   要保持覆蓋類型相同，請選擇 `No Change To <override type>` （預設）。 此設定將保持先前定義的覆蓋值不變。

   - **價格**  — 按一下 **[!UICONTROL Change Listing Price]** 並輸入您的定價值 **[!UICONTROL Price Override]**。
   - **處理時間**  — 按一下 **[!UICONTROL Change Handling Time]** 並輸入定義的時間值（以天為單位） **[!UICONTROL Handling Time Override]**。
   - **條件**  — 按一下 **[!UICONTROL Change Condition]** 並選擇 **[!UICONTROL Condition Override]**。
   - **賣方便箋**  — 按一下 **[!UICONTROL Change Seller Notes]** 並輸入您的備注文本 **[!UICONTROL Seller Notes Override]**。

1. 要刪除覆蓋類型，請按一下 **刪除** 用於要刪除的每種類型。 如果不刪除，則先前定義的值將保留在覆蓋中。

1. 按一下 **[!UICONTROL Save Listing Override]**。

   的 _[!UICONTROL Product Listing Overrides]_頁。 清單的狀態更改為 `Relist in Progress`。 此更改將隨您的下一次資料同步（如您的cron設定中配置）發佈到Amazon。 如果尚未列出，則還會將清單添加到_[!UICONTROL Overrides]_ 頁籤。

依託 _建立覆蓋_ 示例。 以下示例顯示對先前建立的覆蓋的編輯，該覆蓋定義了 `$50`，刪除「處理時間」改寫，並保留以前的「條件」和「賣方附註」改寫。

![編輯或刪除覆蓋](assets/amazon-overrides-edit-2.png)
__

## 編輯或刪除多個清單的覆蓋 {#edit-override-multiple-listings}

的 _[!UICONTROL Edit Listing Overrides]_操作在_[!UICONTROL Inactive]_。 _[!UICONTROL Active]_。_[!UICONTROL Overrides]_, _[!UICONTROL Ineligible]_頁籤。

>[!NOTE]
>
>由於您正在修改多個清單的替代，因此 _[!UICONTROL Listing Details]_修改單個清單時，不會顯示節。

1. 查看上的清單 _[!UICONTROL Products Listings]_頁(P)_[!UICONTROL Inactive]_。 _[!UICONTROL Active]_。_[!UICONTROL Overrides]_, _[!UICONTROL Ineligible]_)的正平方根。

1. 選中要修改的每個清單左側列中的複選框。

1. 下 _[!UICONTROL Actions]_按一下&#x200B;**[!UICONTROL Edit Listing Overrides]**。

   的 _[!UICONTROL Product Listing Overrides]_的上界。

   ![選擇Amazon清單覆蓋](assets/amazon-actions-edit-listing-overrides.png)

1. 編輯 _[!UICONTROL Override]_設定，定義要更改的類型的節（價格、處理時間、條件、賣方附註）。

   要保持覆蓋相同，請選擇 `No Change To <override type>` （預設）。 此設定將保持先前定義的覆蓋值不變。

   - **價格**  — 按一下 **[!UICONTROL Change Listing Price]** 並輸入您的定價值 **[!UICONTROL Price Override]**。
   - **處理時間**  — 按一下 **[!UICONTROL Change Handling Time]** 並輸入定義的時間值（以天為單位） **[!UICONTROL Handling Time Override]**。
   - **條件**  — 按一下 **[!UICONTROL Change Condition]** 並選擇 **[!UICONTROL Condition Override]**。
   - **賣方便箋**  — 按一下 **[!UICONTROL Change Seller Notes]** 並輸入您的備注文本 **[!UICONTROL Seller Notes Override]**。

1. 要刪除覆蓋類型，請按一下 **[!UICONTROL Remove]** 用於要刪除的每種類型。 如果不刪除，則先前定義的值將保留在覆蓋中。

1. 按一下 **[!UICONTROL Save Listing Override]**。

   的 _[!UICONTROL Product Listing Overrides]_頁。 清單的狀態更改為 `Relist in Progress`。 此更改將隨您的下一次資料同步（如您的cron設定中配置）發佈到Amazon。 如果尚未列出，則還會將清單添加到_[!UICONTROL Overrides]_ 頁籤。

### 覆蓋類型

| 覆蓋 | 說明 |
|--- |--- |
| [!UICONTROL Price Override] | 價格覆蓋定義清單的價格。 此覆蓋優先於所有自動設定，直到移除覆蓋。<br><br>要改寫產品價格，請選擇 **[!UICONTROL Change Listing Price]** 並輸入 **[!UICONTROL Price Override]**。 |
| [!UICONTROL Handling Time Override] | 處理時間覆蓋定義處理和發運產品所花費的時間（以天為單位）。 處理時間覆蓋優先於所有自動和預設處理時間設定，直到移除覆蓋。<br><br>中存在的值 _[!UICONTROL Handling Time Override]_框中定義的預設處理時間 [清單設定](./listing-settings.md) 或您定義的覆蓋處理時間。 如果刪除處理時間覆蓋，則清單預設為在清單設定中定義的處理時間。<br><br>要定義處理時間改寫，請選擇&#x200B;**[!UICONTROL Change Handling Time]**並輸入新的處理時間（以天為單位）**[!UICONTROL Handling Time Override]**。 |
| [!UICONTROL Condition Override] | 要覆蓋清單條件，請選擇 **[!UICONTROL Change Condition]** 並選擇新條件 **條件覆蓋**。 |
| [!UICONTROL Seller Notes Override] | 對於目錄中使用非 `New`，可以添加賣家便箋，以進一步詳細說明您的產品及其條件給潛在買家。 您可以為 `New` 條件產品，但Amazon不顯示注釋。<br><br>要改寫賣家附註，請選擇 **[!UICONTROL Change Seller Notes]** 並輸入新附註 **[!UICONTROL Seller Notes Override]**。 |
