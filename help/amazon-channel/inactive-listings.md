---
title: 非活動清單
description: Amazon銷售管道提供[!UICONTROL Inactive]標籤，用於監控您目前不活動的 [!DNL Amazon Marketplace] 清單。
exl-id: 1d20e75f-3346-48cb-83f7-a9e7acb26a96
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# 非活動清單

_[!UICONTROL Inactive]_標籤會顯示已發佈至Amazon但在[!DNL Amazon Marketplace]上未作用的產品。 您的清單可能因一些不同的原因而非使用中。 例如，您可能不符合列出該特定品牌的資格。 非作用中清單由Amazon的清單標準和您的[!DNL Amazon Seller Central]帳戶權限決定。

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL End Listing(s) on Amazon]**:選擇從中刪除所有選定的清 [!DNL Amazon Marketplace]單。請參閱[結束Amazon清單](./end-listings-manually.md)。

- **[!UICONTROL Edit Listing Overrides]**:選擇以更改清單的覆蓋設定。請參閱[覆蓋](./overrides.md)或[編輯或刪除覆蓋](./creating-editing-overrides.md#edit-override-single-listing)。

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL View Details]**：選擇檢視清單詳細資訊，包括 [清單活動記錄](./product-listing-details.md#listing-activity-log)、 [Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和最低 [競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。此動作僅供檢視。 清單詳細資訊中不能進行任何更改。 請參閱[查看詳細資訊](./product-listing-details.md)。

- **[!UICONTROL Create Override]**：選擇建立覆寫並套用至此清單。請參閱[建立覆蓋](./creating-editing-overrides.md)。

- **[!UICONTROL Edit Assigned ASIN]**：選擇以修改指派給目錄產品的ASIN。如果目錄中的產品符合錯誤的ASIN，則會使用此動作。 請參閱[編輯已分配的ASIN](./edit-assigned-asin.md)。

- **[!UICONTROL Create Alias Seller SKU]**：選擇建立別名SKU（庫存保留單位），以便從相同目錄產品建立Amazon清單。請參閱「建立別名賣家SKU](./create-alias-seller-sku.md)」。[

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**：選擇以更改與訂單關聯的履行方法。請參閱[設定履行者設定](./fulfilled-by.md#configure-fulfilled-by-settings)。

- **[!UICONTROL End Listing]**：選擇從中移除清 [!DNL Amazon Marketplace]單。請參閱[結束Amazon清單](./end-listings-manually.md)。

>[!NOTE]
>
>如果您正在處理清單，則頁簽上方會顯示一則訊息，指出清單的數量。

![非作用中Amazon清單](assets/amazon-inactive-listings.png)

Amazon銷售管道首頁共用一些常見的[工作區控制項](./workspace-controls.md)，可讓您自訂顯示的資料。

| 欄 | 說明 |
|--- |--- |
| [!UICONTROL Amazon Seller SKU] | 由Amazon指派給產品的SKU（庫存保管單位），用以識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 10個字母和/或數字的唯一區塊，用於識別項目。<br><br>ASIN代表Amazon標準識別碼。ASIN是10個字母和/或數字的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[條件](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的掛牌價加其運價。 |
| [!UICONTROL Amazon Quantity] | 產品主動列於Amazon時的可用數量。 |
| [!UICONTROL Status] | 清單的狀態，由Amazon定義。 |
| [!UICONTROL Inactive Reason (if provided by Amazon)] | Amazon並不總是提供非作用中清單的原因，您可以聯絡客戶支援以解決清單問題。 在某些情況下，Amazon會通知您原因。 要查看這些響應，請按一下&#x200B;_[!UICONTROL Action]_列中的&#x200B;**[!UICONTROL View Details]**。 如果這些問題已解決，且Amazon移除了錯誤，產品會移至_[!UICONTROL Active]_&#x200B;標籤。 |
| 動作 | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**，然後選取選項：<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[[!UICONTROL Create Override]](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
