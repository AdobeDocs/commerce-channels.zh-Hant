---
title: 依動作管理Amazon產品清單
description: 當您管理Amazon清單時，可以將動作套用至個別或多個清單。
feature: Sales Channels, Products
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 依動作管理Amazon產品清單

_[!UICONTROL Product Listings]_頁面包含數個索引標籤，您可從這些索引標籤檢視所有清單的狀態，並將您的產品與Amazon清單比對。

可用的清單工作在每個索引標籤上稍有不同，但[工作區控制項](./workspace-controls.md)相同，可讓您自訂清單顯示的資料。

**[!UICONTROL Actions]**&#x200B;下的選項可以將動作套用至多個清單，而&#x200B;_[!UICONTROL Action]_欄中&#x200B;**[!UICONTROL Select]**下的選項僅會將動作套用至個別清單。

另請參閱[依狀態管理清單/標籤](./managing-listings-by-tab.md)。

| 動作 | 說明 | 索引標籤 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | 用於透過比對程式將不完整產品移回。 若要嘗試重新比對，您必須修改您的[清單](./listing-settings.md)和[目錄搜尋](./catalog-search.md)設定，以增加自動比對的可能性。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | 選取要比對的清單、輸入要比對的ASIN或指派缺少的條件，手動比對目錄產品與Amazon清單。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | 檢視使用中產品的其他資訊，包括清單活動記錄，其中顯示個別SKU /產品的變更。 | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | 使用隨Amazon清單匯入的資訊建立[!DNL Commerce]目錄產品。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| 嘗試自動比對 | 根據搜尋條件設定，嘗試自動比對您的[!DNL Commerce]目錄與Amazon清單。 若要嘗試重新比對，您必須修改您的[清單](./listing-settings.md)和[目錄搜尋](./catalog-search.md)設定，以增加自動比對的可能性。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | 手動選取您[!DNL Commerce]目錄中的現有產品，並將其指派給Amazon清單。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | 使用隨Amazon清單匯入的資訊建立[!DNL Commerce]目錄產品。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | （整批動作）用於重新列出已結束的清單，或手動列出符合清單規則資格的產品，但您的&#x200B;_[!UICONTROL Product Listing Actions]_未設定為`Automatically list new products`。 | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | （單一清單動作）用於重新列出已結束的清單。 此動作也用於在&#x200B;_[!UICONTROL Product Listing Actions]_未設定為`Automatically list new products`時，手動列出符合您清單規則資格的產品。 | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | （整批動作）用於手動結束與移除Amazon上現有產品的清單。 已結束的清單只要符合您的清單規則資格，就可以重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | （整批作業）手動編輯現有的「覆寫」，以設定個別清單的價格、處理時間、條件和賣家備註文字，忽略其他清單預設值、設定及規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | 手動建立「覆寫」，針對個別清單設定價格、處理時間、條件和賣家備註文字，忽略其他清單預設值、設定及規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | 用於與目錄產品相符的ASIN必須修改時（例如：產品與錯誤的清單ASIN相符）。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | 可提供兩種功能：<br><br>可用來在目錄產品與兩個Amazon清單之間建立一對二的關係。 範例： Amazon的產品以不同的ASIN值列出。 您可以將一個目錄產品與產品的兩個ASIN清單比對。<br><br>可用於控制不同Amazon地區的清單。 範例：您的型錄產品有根據Amazon地區（美國地區為FBA，加拿大地區為FBM）定義的不同送貨方法。 若要控制庫存/數量，您可以建立別名賣方SKU，然後使用不同的賣方SKU重新列出該區域的相同產品。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | 用於修改與產品相關的履行方式(由Amazon履行：FBA或由商家履行：FBM)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | （單一清單動作）用於手動結束Amazon上現有產品的清單，並將其移除。 已結束的清單只要符合您的清單規則資格，就可以重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | （單一清單動作）手動編輯現有的「覆寫」，以設定個別清單的價格、處理時間、條件和賣家附註文字，忽略其他清單預設值、設定及規則。 | [[!UICONTROL Overrides]](./overrides.md) |

## 存取產品清單

1. 在&#x200B;_管理員_&#x200B;側邊欄上，前往&#x200B;**行銷** > _管道_ > **AmazonSales Channel**。

1. 按一下商店卡片上的&#x200B;**檢視商店**。

1. 在商店儀表板上，按一下&#x200B;_商店清單_&#x200B;區段中的&#x200B;**管理清單**。
