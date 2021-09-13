---
title: 不合格清單
description: Amazon銷售管道提供[!UICONTROL Ineligible]標籤，協助您根據目前的上市規則管理不符合清單資格的項目。
exl-id: ae63898d-ff5c-43eb-b759-5bc80829d4d4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 不符合資格的清單

_[!UICONTROL Ineligible]_標籤會顯示目前已在Amazon上發佈，但根據您目前的上市規則，不符合上市資格的所有產品清單。 如果先前的產品符合條件，且清單規則已修改為使其現在不合格，則與產品相關聯的數量會降為0，而產品標籤為_&#x200B;不合格&#x200B;_。 不過，它仍存在於您的[!DNL Amazon Seller Account]上。

若要將產品移出&#x200B;_[!UICONTROL Ineligible]_標籤，您可以[修改清單規則](./listing-rules.md)，讓您的產品符合資格。

_[!UICONTROL Ineligible]_標籤上的可用操作包括：

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL End Listing(s) on Amazon]**:選擇從中刪除所有選定的清 [!DNL Amazon Marketplace]單。請參閱[結束Amazon清單](./end-listings-manually.md)。

- **[!UICONTROL Edit Listing Overrides]**:選擇以更改清單的覆蓋設定。請參閱[覆蓋](./overrides.md)或[編輯或刪除覆蓋](./creating-editing-overrides.md#edit-override-single-listing)。

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL View Details]**：選擇檢視清單詳細資訊，包括 [清單活動記錄](./product-listing-details.md#listing-activity-log)、 [Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和最低 [競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。此動作僅供檢視。 清單詳細資訊中不能進行任何更改。 請參閱[查看詳細資訊](./product-listing-details.md)。

- **[!UICONTROL Create Override]**：選擇建立覆寫並套用至此清單。請參閱[建立覆蓋](./creating-editing-overrides.md)。

- **[!UICONTROL Edit Assigned ASIN]**：選擇以修改指派給目錄產品的ASIN。如果目錄中的產品符合錯誤的ASIN，則會使用此動作。 請參閱[編輯已分配的ASIN](./edit-assigned-asin.md)。

- **[!UICONTROL Create Alias Seller SKU]**：選擇建立別名SKU，以便從相同目錄產品建立Amazon清單。請參閱「建立別名賣家SKU](./create-alias-seller-sku.md)」。[

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**：選擇以更改與訂單關聯的履行方法。請參閱[設定履行者設定](./fulfilled-by.md#configure-fulfilled-by-settings)。

- **[!UICONTROL End Listing]**：選擇從中移除清 [!DNL Amazon Marketplace]單。請參閱[結束Amazon清單](./end-listings-manually.md)。

>[!NOTE]
>如果正在處理清單，則清單數將顯示在頁簽上方的消息中。

![不符合資格的Amazon清單](assets/amazon-ineligible-listings.png)

Amazon銷售管道首頁共用一些常見的[工作區控制項](./workspace-controls.md)，可讓您自訂顯示的資料。

## 預設列

| 欄 | 說明 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 由Amazon指派給產品的SKU（庫存保管單位），用以識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 10個字母和/或數字的唯一區塊，用於識別項目。<br><br>ASIN代表 [!DNL Amazon Standard Identification Number]。ASIN是10個字母和/或數字的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[條件](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的掛牌價加其運價。 |
| [!UICONTROL Amazon Quantity] | 產品主動列於Amazon時的可用數量。 |
| [!UICONTROL Action] | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**，然後選取選項：<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[建立覆蓋](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
