---
title: 非作用中的Amazon清單
description: Amazon sales channel提供[!UICONTROL Inactive]索引標籤，以監視您目前非作用中的 [!DNL Amazon Marketplace] 清單。
feature: Sales Channels, Products
exl-id: 1d20e75f-3346-48cb-83f7-a9e7acb26a96
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# 非作用中的Amazon清單

_[!UICONTROL Inactive]_索引標籤會顯示您已發佈至Amazon但於[!DNL Amazon Marketplace]上未啟用的產品。 您的清單可能由於幾個不同原因而處於非使用中狀態。 例如，您可能有資格列出該特定品牌。 非作用中清單是由Amazon的清單標準和您的[!DNL Amazon Seller Central]帳戶許可權所指定。

在&#x200B;_[!UICONTROL Actions]_下：

- **[!UICONTROL End Listing(s) on Amazon]**：選擇從[!DNL Amazon Marketplace]移除所有選取的清單。 請參閱[結束Amazon清單](./end-listings-manually.md)。

- **[!UICONTROL Edit Listing Overrides]**：選擇以變更清單的覆寫設定。 請參閱[覆寫](./overrides.md)或[編輯或移除覆寫](./creating-editing-overrides.md#edit-override-single-listing)。

在&#x200B;_[!UICONTROL Action]_欄的&#x200B;**[!UICONTROL Select]**下：

- **[!UICONTROL View Details]**：選擇檢視清單詳細資料，包括[清單活動記錄](./product-listing-details.md#listing-activity-log)、[Buy Box競爭者定價](./product-listing-details.md#buy-box-competitor-pricing)和[最低競爭者定價](./product-listing-details.md#lowest-competitor-pricing)。 此動作僅供檢視。 清單詳細資料不可變更。 檢視[檢視詳細資料](./product-listing-details.md)。

- **[!UICONTROL Create Override]**：選擇建立覆寫並將其套用至此清單。 請參閱[建立覆寫](./creating-editing-overrides.md)。

- **[!UICONTROL Edit Assigned ASIN]**：選擇修改指派給目錄產品的ASIN。 如果目錄中的產品符合錯誤的ASIN，則會使用此動作。 請參閱[編輯指派的ASIN](./edit-assigned-asin.md)。

- **[!UICONTROL Create Alias Seller SKU]**：選擇建立別名SKU （庫存單位），此別名SKU可用來從相同目錄產品建立Amazon清單。 請參閱[建立別名賣家SKU](./create-alias-seller-sku.md)。

- **[!UICONTROL Switch to Fulfilled by Amazon/Merchant]**：選擇變更與訂單相關聯的履行方法。 請參閱[設定完成者設定](./fulfilled-by.md#configure-fulfilled-by-settings)。

- **[!UICONTROL End Listing]**：選擇從[!DNL Amazon Marketplace]移除清單。 請參閱[結束Amazon清單](./end-listings-manually.md)。

>[!NOTE]
>
>如果您有處理中的清單，標籤上方會出現一則訊息，指出清單數目。

![非作用中的Amazon清單](assets/amazon-inactive-listings.png){width="600" zoomable="yes"}

Amazon sales channel首頁共用一些常見的[工作區控制項](./workspace-controls.md)，可讓您自訂顯示的資料。

| 欄 | 說明 |
|------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Amazon Seller SKU] | Amazon指派給產品的SKU （庫存單位），用於識別產品、選項、價格和製造商。 |
| [!UICONTROL ASIN] | 識別專案的10個字母和/或數字的唯一區塊。<br><br>ASIN代表Amazon標準識別碼。 ASIN是識別專案的10個字母和/或數字的唯一區塊。 對於書籍，ASIN與ISBN編號相同，但對於所有其他產品，當專案上傳到它們的目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資料頁面上找到專案ASIN，以及與此專案相關的其他詳細資料。 |
| [!UICONTROL Product Listing Name] | 產品的名稱。 |
| [!UICONTROL Condition] | 產品的[狀況](./product-listing-condition.md)。 |
| [!UICONTROL Landed Price] | 產品的上市價格加上其送貨價格。 |
| [!UICONTROL Amazon Quantity] | 產品在Amazon上主動列出時的可用數量。 |
| [!UICONTROL Status] | 清單的狀態，由Amazon定義。 |
| [!UICONTROL Inactive Reason (if provided by Amazon)] | Amazon不一定會提供不活躍清單的原因，您可以聯絡客戶支援以解決清單問題。 在某些情況下，Amazon會通知您原因。 若要檢視這些回應，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL View Details]**。 如果這些問題已解決且Amazon已移除錯誤，產品會移至_[!UICONTROL Active]_&#x200B;標籤。 |
| 動作 | 可套用至特定清單的可用動作清單。 若要套用動作，請按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Select]**並選取選項：<ul><li>[[!UICONTROL View Details]](./product-listing-details.md)</li><li>[[!UICONTROL Create Override]](./creating-editing-overrides.md)</li><li>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)</li><li>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)</li><li>[[!UICONTROL Switch to Fulfilled By Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings)</li><li>[[!UICONTROL End Listing]](./end-listings-manually.md)</li></ul> |
