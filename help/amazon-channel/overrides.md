---
title: 覆蓋
description: AmazonSales Channel提供「覆蓋」頁籤，幫助您識別和管理在Amazon清單中應用覆蓋的方式。
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# 覆蓋

的 _[!UICONTROL Overrides]_頁籤顯示已應用替代的Amazon清單。 覆蓋是清單特定的設定，可以將定義的值設定為清單。 應用於清單的覆蓋定義清單的設定，而不考慮其他定義的清單設定或清單適合的規則。 當將覆蓋應用於清單時，清單將出現在_[!UICONTROL Overrides]_ 頁籤。 覆蓋中定義的值將出現在清單的相應列中。 可應用的替代有四種類型：價格、處理時間、條件和銷售者票據。

## 覆蓋類型

| 類型 | 說明 |
|---|---|
| 價格 | 設定清單價格的覆蓋，忽略清單的所有其他價格設定。 <br><br>**示例**:您已定義了適用於目錄特定類別中所有產品的20%折扣價格規則。 您擁有新的產品，而且需求很高，因此即使產品屬於該類別，您也不希望將折扣價格應用於該清單。 您可以選擇清單， [建立價格改寫](./creating-editing-overrides.md#edit-override-single-listing)，並在價格覆蓋中定義清單價格。 |
| 處理時間 | 設定清單處理時間的覆蓋，忽略清單設定中設定的預設處理時間。<br><br>**示例**:清單的預設處理時間設定為2天。 您的產品很脆弱，需要額外的一天來確保其特殊包裝用於運輸。 你可以查看清單， [建立處理時間覆蓋](./creating-editing-overrides.md#edit-override-single-listing)，並定義三天的處理時間。<br><br>**注：** 對於設定為的產品不可用 `Fulfilled by Amazon`。 |
| 條件 | 設定清單條件值的覆蓋，而不考慮分配給清單的條件屬性。<br><br>**示例**:目錄中的大多數產品都是新產品，但您的產品是已翻新的產品。 你可以查看清單， [建立條件覆蓋](./creating-editing-overrides.md#edit-override-single-listing)，並定義清單的「已翻新」條件。<br><br>**注：** 對於設定為的產品不可用 `Fulfilled by Amazon`。 |
| 賣方便箋 | 定義 _賣方便箋_ 的下界。 此欄位可用於添加與產品或所應用的覆蓋相關的附加資訊，通常用於描述「非新」產品的狀況。 此欄位中的文本與購物者的清單一起顯示。 無法為條件值為的清單添加賣方票據 `New`。 <br><br>**示例**:你的產品 `Refurbished` 的子菜單。 通常情況下，此條件下的產品不包括任何手冊或文檔，但您有其他供應商提供此產品，其中包括手冊。 你可以查看清單， [建立賣家便箋覆蓋](./creating-editing-overrides.md#edit-override-single-listing)，並添加此手冊清單中唯一的文本注釋，以便購物者知道其中包含該手冊。<br><br>**注釋**:如果產品具有定義的條件 `New`，您可以輸入賣方便箋改寫，但Amazon不顯示 `New` 產品。 |

可以建立、編輯或刪除 [單一清單](./creating-editing-overrides.md#edit-override-single-listing)。 在 _[!UICONTROL Inactive]_。_[!UICONTROL Active]_, _[!UICONTROL Ineligible]_頁籤，可按一下&#x200B;**[!UICONTROL Select]**的_[!UICONTROL Action]_ 列和選擇 **[!UICONTROL Create Override]**。 的 _[!UICONTROL Edit Overrides]_僅當清單已應用覆蓋並在_[!UICONTROL Overrides]_ 頁籤。

也可以建立、編輯或刪除覆蓋，以 [多個清單](./creating-editing-overrides.md#edit-override-multiple-listings)。 在 _[!UICONTROL Inactive]_。_[!UICONTROL Active]_, _[!UICONTROL Ineligible]_頁籤，可按一下&#x200B;**[!UICONTROL Select]**的_[!UICONTROL Action]_ 列和選擇 **[!UICONTROL Edit Listing Overrides]**。

刪除覆蓋將指示清單使用清單設定和規則定義的值。

在定義改寫時，您還可以選擇輸入單個改寫類型或這些類型的任何組合。

請參閱 [建立和編輯覆蓋](./creating-editing-overrides.md)。

>[!NOTE]
>
>如果正在處理清單，則清單數將顯示在頁籤上方的消息中。

![「覆蓋」頁籤](assets/amazon-overrides.png)

Amazon銷售渠道首頁共用一些共同的 [工作區控制項](./workspace-controls.md) 允許您自定義顯示的資料。

## 預設列

| 列 | 說明 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 由Amazon分配給產品的SKU（庫存單位），以標識產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 標識項的10個字母和/或數字的唯一塊。<br><br>ASIN代表Amazon標準標識號。 ASIN是由10個字母和/或數字組成的唯一塊，用於標識項目。 對於書籍，ASIN與ISBN號相同，但對於所有其他產品，在將項目上載到其目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Condition Override] | 覆蓋中定義的新條件。 如果應用於清單的覆蓋不是條件覆蓋， `Not Selected` 列中。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Seller Notes Override] | 覆蓋中定義的新賣方注釋。 如果應用於清單的覆蓋不是此類覆蓋，則此列為空。 |
| [!UICONTROL Handling Override] | 覆蓋中定義的新處理時間（以天為單位）。 如果應用於清單的覆蓋不是處理時間覆蓋，則此列為空。 |
| [!UICONTROL List Price Override] | 覆蓋中定義的新上市價格。 如果應用於清單的改寫不是價格改寫， `N/A` 列中。 |
| [!UICONTROL Action] | 可應用於特定清單的可用操作的清單。 要應用操作，請在 _[!UICONTROL Action]_列，按一下&#x200B;**[!UICONTROL Select]**，然後選擇：<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
