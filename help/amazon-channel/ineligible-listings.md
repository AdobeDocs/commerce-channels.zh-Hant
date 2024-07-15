---
title: 不符合資格的Amazon清單
description: Amazon sales channel提供[!UICONTROL Ineligible]標籤，可協助您管理不符合目前清單規則條件的專案。
feature: Sales Channels, Products
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 不符合資格的Amazon清單

_[!UICONTROL Ineligible]_索引標籤會顯示目前在Amazon上發佈但根據您目前的清單規則不符合清單資格的所有產品清單。 如果先前產品符合資格，且清單規則已修改為現在不符合資格，則與產品相關的數量會降至0，而產品會標示為_&#x200B;不符合&#x200B;_。 但是，它仍存在於您的[!DNL Amazon Seller Account]上。

若要將產品移出&#x200B;_[!UICONTROL Ineligible]_標籤，您可以[修改您的清單規則](./listing-rules.md)，讓您的產品符合資格。

_[!UICONTROL Ineligible]_標籤上的可用動作包括：

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL End Listing(s) on Amazon]**：選擇從[!DNL Amazon Marketplace]移除所有選取的清單。 請參閱[結束Amazon清單](./end-listings-manually.md)。

- **[!UICONTROL Edit Listing Overrides]**：選擇以變更清單的覆寫設定。 請參閱[覆寫](./overrides.md)或[編輯或移除覆寫](./creating-editing-overrides.md#edit-override-single-listing)。

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL View Details]**：選擇檢視清單詳細資料，包括[清單活動記錄](./product-listing-details.md#listing-activity-log)、[Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和[最低競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。 此動作僅供檢視。 清單詳細資料不可變更。 檢視[檢視詳細資料](./product-listing-details.md)。

- **[!UICONTROL Create Override]**：選擇建立覆寫並將其套用至此清單。 請參閱[建立覆寫](./creating-editing-overrides.md)。

- **[!UICONTROL Edit Assigned ASIN]**：選擇修改指派給目錄產品的ASIN。 如果目錄中的產品符合錯誤的ASIN，則會使用此動作。 請參閱[編輯指派的ASIN](./edit-assigned-asin.md)。

- **[!UICONTROL Create Alias Seller SKU]**：選擇建立別名SKU，此SKU可用來從相同目錄產品建立Amazon清單。 請參閱[建立別名賣家SKU](./create-alias-seller-sku.md)。

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**：選擇變更與訂單相關聯的履行方法。 請參閱[設定完成者設定](./fulfilled-by.md#configure-fulfilled-by-settings)。

- **[!UICONTROL End Listing]**：選擇從[!DNL Amazon Marketplace]移除清單。 請參閱[結束Amazon清單](./end-listings-manually.md)。

>[!NOTE]
>如果您有處理中的清單，清單的數量會顯示在標籤上方的訊息中。

![不符合資格的Amazon清單](assets/amazon-ineligible-listings.png){width="600" zoomable="yes"}

Amazon sales channel首頁共用一些常見的[工作區控制項](./workspace-controls.md)，可讓您自訂顯示的資料。

## 預設欄

| 欄 | 說明 |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Amazon指派給產品的SKU （庫存單位），用於識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 識別專案的10個字母和/或數字的唯一區塊。<br><br>ASIN代表[!DNL Amazon Standard Identification Number]。 ASIN是識別專案的10個字母和/或數字的唯一區塊。 對於書籍，ASIN與ISBN編號相同，但對於所有其他產品，當專案上傳到它們的目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資料頁面上找到專案ASIN，以及與此專案相關的其他詳細資料。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[狀況](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的上市價格加上其送貨價格。 |
| [!UICONTROL Amazon Quantity] | 產品在Amazon上主動列出時的可用數量。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**並選取選項：<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[建立覆寫](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
