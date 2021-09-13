---
title: 按操作管理產品清單
description: 當您管理Amazon清單時，可以將動作套用至個別或多個清單。
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 依動作管理產品清單

_[!UICONTROL Product Listings]_頁面包含數個索引標籤，您可從這些索引標籤檢視所有清單的狀態，並將產品與Amazon清單相符。

每個標籤上可用的清單任務稍有不同，但[workspace控制項](./workspace-controls.md)是相同的，允許您自訂顯示清單的資料。

**[!UICONTROL Actions]**&#x200B;下的選項可以將操作應用於多個清單，而&#x200B;_[!UICONTROL Action]_列中&#x200B;**[!UICONTROL Select]**下的選項僅將操作應用於單個清單。

另請參閱[依狀態管理清單/ Tab](./managing-listings-by-tab.md)。

| 動作 | 說明 | 標籤 |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | 用於在匹配流程中將不完整的產品移回。 若要嘗試重新匹配，您必須修改[Listing](./listing-settings.md)和[Catalog Search](./catalog-search.md)設定，以增加自動匹配的可能性。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | 選取要比對的清單、輸入要比對的ASIN或指派缺少的條件，以手動比對目錄產品與Amazon清單。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | 檢視您作用中產品的其他資訊，包括清單活動記錄，其中會顯示個別SKU/產品的變更。 | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | 使用從Amazon清單匯入的資訊建立[!DNL Commerce]目錄產品。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| 嘗試自動匹配 | 根據搜尋條件設定，嘗試在[!DNL Commerce]目錄和Amazon清單之間自動比對。 若要嘗試重新匹配，您必須修改[Listing](./listing-settings.md)和[Catalog Search](./catalog-search.md)設定，以增加自動匹配的可能性。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | 手動選取[!DNL Commerce]目錄中的現有產品，並將其指派至Amazon清單。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | 使用從Amazon清單匯入的資訊建立[!DNL Commerce]目錄產品。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | （成批活動）用於重新列出已結束的清單，或人工列出符合您的清單規則資格的產品，但您的&#x200B;_[!UICONTROL Product Listing Actions]_未設定為`Automatically list new products`。 | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | （單一清單動作）用於重新列出已結束的清單。 當&#x200B;_[!UICONTROL Product Listing Actions]_未設為`Automatically list new products`時，此動作還用於手動列出符合您的清單規則資格的產品。 | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | （成批活動）用於手動結束和移除您產品上存在Amazon的清單。 只要已結束的清單符合您的上市規則資格，就可將其重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | （成批活動）人工編輯現有的「改寫」，該改寫設定單個清單的價格、處理時間、條件和賣方附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | 手動建立「覆蓋」，該覆蓋設定單個清單的價格、處理時間、條件和賣方附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | 如果必須修改與目錄產品相符的ASIN，則使用(範例：如果產品與錯誤的清單ASIN匹配)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | 可提供兩個函式：<br><br>可用來在目錄產品與兩個Amazon清單之間建立1對2關係。 範例：Amazon列出的產品具有不同的ASIN值。 您可以將一個目錄產品與產品的兩個ASIN清單匹配。<br><br>可用來控制不同Amazon地區的清單。範例：您有一個目錄產品，其根據Amazon地區定義了不同的運送方法（美國地區為FBA，加拿大地區為FBM）。 若要控制庫存/數量，您可以建立別名賣家SKU，並將該地區中的相同產品重新列出為不同的賣家SKU。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | 用於修改與您的產品相關聯的履行方法(由Amazon履行：FBA或由商家履行：FBM)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | （單一清單動作）用於手動結束和移除您產品上存在Amazon的清單。 只要已結束的清單符合您的上市規則資格，就可將其重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | （單一清單活動）手動編輯現有的「覆蓋」，該覆蓋設定單個清單的價格、處理時間、條件和賣方附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Overrides]](./overrides.md) |

## 存取產品清單

1. 在&#x200B;_Admin_&#x200B;側欄上，前往&#x200B;**行銷** > _頻道_ > **AmazonSales Channel**。

1. 按一下儲存卡上的&#x200B;**檢視儲存**。

1. 在儲存控制面板上，按一下&#x200B;_儲存清單_&#x200B;區段中的&#x200B;**管理清單**。
