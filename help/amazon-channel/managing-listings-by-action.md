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

此 _[!UICONTROL Product Listings]_頁面包含數個標籤，您可從中檢視所有清單的狀態，並將產品與Amazon清單配對。

每個標籤上可用的清單任務稍有不同，但 [工作區控制項](./workspace-controls.md) 相同，可讓您自訂為清單顯示的資料。

下方的選項 **[!UICONTROL Actions]** 可將動作套用至多個清單，而 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄僅將動作套用至個別清單。

另請參閱 [按狀態/頁簽管理清單](./managing-listings-by-tab.md).

| 動作 | 說明 | 標籤 |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | 用於在匹配流程中將不完整的產品移回。 若要嘗試重新比對，您必須修改 [清單](./listing-settings.md) 和 [目錄搜尋](./catalog-search.md) 設定以增加自動比對的可能。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | 選取要比對的清單、輸入要比對的ASIN或指派缺少的條件，以手動比對目錄產品與Amazon清單。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | 檢視您作用中產品的其他資訊，包括清單活動記錄，其中會顯示個別SKU/產品的變更。 | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | 建立 [!DNL Commerce] 使用隨Amazon清單匯入的資訊編錄產品。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| 嘗試自動匹配 | 嘗試在 [!DNL Commerce] 目錄和您的Amazon清單（根據搜尋條件設定）。 若要嘗試重新比對，您必須修改 [清單](./listing-settings.md) 和 [目錄搜尋](./catalog-search.md) 設定以增加自動比對的可能。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | 在您的 [!DNL Commerce] 目錄並指派給Amazon清單。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | 建立 [!DNL Commerce] 使用隨Amazon清單匯入的資訊編錄產品。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | （成批活動）用於重新列出已結束的清單，或人工列出符合您的清單規則資格但您的 _[!UICONTROL Product Listing Actions]_未設為 `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | （單一清單動作）用於重新列出已結束的清單。 此動作也可用來手動列出符合上市規則資格的產品，當 _[!UICONTROL Product Listing Actions]_未設為 `Automatically list new products`. | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | （成批活動）用於手動結束和移除您產品上存在Amazon的清單。 只要已結束的清單符合您的上市規則資格，就可將其重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | （成批活動）人工編輯現有的「改寫」，該改寫設定單個清單的價格、處理時間、條件和賣方附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | 手動建立「覆蓋」，該覆蓋設定單個清單的價格、處理時間、條件和賣方附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | 如果必須修改與目錄產品相符的ASIN，則使用(範例：如果產品與錯誤的清單ASIN匹配)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | 可提供兩種功能：<br><br>可用來在目錄產品和兩個Amazon清單之間建立1對2關係。 範例：Amazon列出的產品具有不同的ASIN值。 您可以將一個目錄產品與產品的兩個ASIN清單匹配。<br><br>可用來控制不同Amazon地區的清單。 範例：您有一個目錄產品，其根據Amazon地區定義了不同的運送方法（美國地區為FBA，加拿大地區為FBM）。 若要控制庫存/數量，您可以建立別名賣家SKU，並將該地區中的相同產品重新列出為不同的賣家SKU。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | 用於修改與您的產品相關聯的履行方法(由Amazon履行：FBA或由商家履行：FBM)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | （單一清單動作）用於手動結束和移除您產品上存在Amazon的清單。 只要已結束的清單符合您的上市規則資格，就可將其重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | （單一清單活動）手動編輯現有的「覆蓋」，該覆蓋設定單個清單的價格、處理時間、條件和賣方附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Overrides]](./overrides.md) |

## 存取產品清單

1. 在 _管理_ 邊欄，轉到 **行銷** > _管道_ > **AmazonSales Channel**.

1. 按一下 **檢視商店** 在商店卡上。

1. 在商店控制面板上，按一下 **管理清單** 在 _儲存清單_ 區段。
