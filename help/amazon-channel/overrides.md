---
title: 覆寫
description: AmazonSales Channel提供「覆寫」標籤，協助您識別及管理如何在Amazon清單中套用覆寫。
exl-id: e31bbbf9-b20d-42fd-a419-93d596e40be2
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# 覆寫

此 _[!UICONTROL Overrides]_標籤會顯示您已套用覆寫的Amazon清單。 覆蓋是清單特定的設定，可用來將定義值設定為清單。 套用至清單的覆寫會定義清單的設定，而不論其他已定義的清單設定或符合清單資格的規則。 將覆蓋應用於清單時，清單會顯示在_[!UICONTROL Overrides]_ 標籤。 在覆蓋中定義的值將顯示在清單的相應列中。 可套用四種覆寫類型：價格、處理時間、條件和賣方票據。

## 覆蓋類型

| 類型 | 說明 |
|---|---|
| 價格 | 設定上市價格的覆寫，會忽略上市的所有其他價格設定。 <br><br>**範例**:您已定義了適用於目錄特定類別中所有產品的20%折扣價格規則。 您的產品是市場新產品，需求很高，因此您不希望將折扣價格套用至清單，即使產品屬於該類別亦然。 您可以選取清單， [建立價格改寫](./creating-editing-overrides.md#edit-override-single-listing)，並定義價格覆寫中的清單價格。 |
| 處理時間 | 設定清單處理時間的覆蓋，忽略清單設定中設定的預設處理時間。<br><br>**範例**:清單的預設處理時間設為2天。 你的產品很脆弱，需要額外的一天來確保其特殊的包裝用於運輸。 您可以檢視清單， [建立處理時間覆蓋](./creating-editing-overrides.md#edit-override-single-listing)，並定義三天的處理時間。<br><br>**注意：** 對於設為的產品不可用 `Fulfilled by Amazon`. |
| 條件 | 設定清單條件值的覆蓋，而不考慮指派給清單的條件屬性。<br><br>**範例**:目錄中的大多數產品是「新條件」，但您的產品是「翻新」狀態。 您可以檢視清單， [建立條件覆寫](./creating-editing-overrides.md#edit-override-single-listing)，並定義清單的「翻新」條件。<br><br>**注意：** 對於設為的產品不可用 `Fulfilled by Amazon`. |
| 賣家筆記 | 定義 _賣家筆記_ 的部分。 此欄位可用來新增與產品或套用的覆寫相關的其他資訊，通常用於說明「非新」產品的條件。 此欄位中的文字會隨購物者的清單顯示。 無法為條件值為的清單添加賣方票據 `New`. <br><br>**範例**:您的產品 `Refurbished` 條件。 通常情況下，此條件下的產品不包含任何手冊或文檔，但您有不同的供應商，該供應商包含手冊。 您可以檢視清單， [建立賣方附註改寫](./creating-editing-overrides.md#edit-override-single-listing)，並新增此清單中關於手冊的唯一文字附註，讓購物者知道其中已包含。<br><br>**附註**:如果產品已定義條件 `New`，您可以輸入賣方附註改寫，但Amazon不會顯示 `New` 產品。 |

您可以建立、編輯或移除 [單一清單](./creating-editing-overrides.md#edit-override-single-listing). 在 _[!UICONTROL Inactive]_,_[!UICONTROL Active]_，和 _[!UICONTROL Ineligible]_索引標籤，您可以按一下&#x200B;**[!UICONTROL Select]**在_[!UICONTROL Action]_ 欄，選擇 **[!UICONTROL Create Override]**. 此 _[!UICONTROL Edit Overrides]_僅當清單已套用覆寫且在_[!UICONTROL Overrides]_ 標籤。

您也可以建立、編輯或移除覆寫，以 [多個清單](./creating-editing-overrides.md#edit-override-multiple-listings). 在 _[!UICONTROL Inactive]_,_[!UICONTROL Active]_，和 _[!UICONTROL Ineligible]_索引標籤，您可以按一下&#x200B;**[!UICONTROL Select]**在_[!UICONTROL Action]_ 欄，選擇 **[!UICONTROL Edit Listing Overrides]**.

移除覆寫會告訴清單使用清單設定和規則所定義的值。

定義覆蓋時，您也可以選擇輸入單個類型的覆蓋或任何類型的組合。

請參閱 [建立和編輯覆蓋](./creating-editing-overrides.md).

>[!NOTE]
>
>如果正在處理清單，則清單數將顯示在頁簽上方的消息中。

![覆蓋頁簽](assets/amazon-overrides.png)

Amazon銷售管道首頁有一些共同之處 [工作區控制項](./workspace-controls.md) 可讓您自訂顯示的資料。

## 預設列

| 欄 | 說明 |
|---|---|
| [!UICONTROL Amazon Seller SKU] | 由Amazon指派給產品的SKU（庫存保管單位），用以識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 10個字母和/或數字的唯一區塊，用於識別項目。<br><br>ASIN代表Amazon標準識別碼。 ASIN是10個字母和/或數字的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Condition Override] | 覆寫中定義的新條件。 如果套用至清單的覆寫不是條件覆寫， `Not Selected` 會出現在此欄中。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Seller Notes Override] | 在置換中定義的新賣方注釋。 如果套用至清單的覆寫不是此類型的覆寫，則此欄為空白。 |
| [!UICONTROL Handling Override] | 在覆蓋中定義的新處理時間（以天為單位）。 如果應用於清單的覆蓋不是處理時間覆蓋，則此列為空。 |
| [!UICONTROL List Price Override] | 覆蓋中定義的新上市價格。 如果應用於清單的改寫不是價格改寫， `N/A` 會出現在此欄中。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請在 _[!UICONTROL Action]_欄，按一下&#x200B;**[!UICONTROL Select]**並選擇選項：<ul><li>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md#edit-override-single-listing)</li><li>[[!UICONTROL View Details]](./product-listing-details.md)</li></ul> |
