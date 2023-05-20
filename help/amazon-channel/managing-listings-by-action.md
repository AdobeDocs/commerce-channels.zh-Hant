---
title: 按操作管理產品清單
description: 在管理Amazon清單時，您可以將操作應用於單個或多個清單。
exl-id: 1cbf16fb-15eb-484b-bea7-28017a0d0c60
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# 按操作管理產品清單

的 _[!UICONTROL Product Listings]_頁面包含多個頁籤，您可以從中查看所有清單的狀態，並將產品與Amazon清單匹配。

每個頁籤上可用的清單任務略有不同，但 [工作區控制項](./workspace-controls.md) 相同，允許您自定義為清單顯示的資料。

選項 **[!UICONTROL Actions]** 可以將操作應用於多個清單，同時 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_列將操作僅應用於單個清單。

另請參閱 [按狀態/頁籤管理清單](./managing-listings-by-tab.md)。

| 操作 | 說明 | 頁籤 |
|--- |--- |--- |
| [[!UICONTROL Re-attempt auto match to Amazon Listing]](./amazon-manually-update-incomplete-listing.md#update-required-info-unable-to-assign-to-amazon-listing) | 用於在匹配流程中移回未完成的產品。 要嘗試重新匹配，必須修改 [清單](./listing-settings.md) 和 [目錄搜索](./catalog-search.md) 設定以增加自動匹配的可能性。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md) | 通過選擇要匹配的清單、輸入要匹配的ASIN或分配缺少的條件，手動將目錄產品與Amazon清單匹配。 | [[!UICONTROL Incomplete]](./incomplete-listings.md) |
| [[!UICONTROL View Details]](./product-listing-details.md) | 查看有關您的活動產品的其他資訊，包括清單活動日誌，其中顯示對單個SKU/產品的更改。 | [[!UICONTROL Incomplete]](./incomplete-listings.md)<br>[[!UICONTROL New Third Party]](./new-third-party-listings.md)<br>[[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md) | 建立 [!DNL Commerce] 使用隨Amazon清單導入的資訊對產品進行編目。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| 嘗試自動匹配 | 嘗試在您的 [!DNL Commerce] 目錄和您的Amazon清單。 要嘗試重新匹配，必須修改 [清單](./listing-settings.md) 和 [目錄搜索](./catalog-search.md) 設定以增加自動匹配的可能性。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md) | 在您的 [!DNL Commerce] 編錄，並分配給Amazon。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md) | 建立 [!DNL Commerce] 使用隨Amazon清單導入的資訊對產品進行編目。 | [[!UICONTROL New Third Party]](./new-third-party-listings.md) |
| [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md) | （成批活動）用於重新列出已結束的清單或人工列出符合上市規則資格的產品，但您 _[!UICONTROL Product Listing Actions]_未設定為 `Automatically list new products`。 | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Publish On Amazon]](./publish-listings-manually.md) | （單個清單操作）用於重新列出已結束的清單。 此操作還用於在以下情況下手動列出符合上市規則資格的產品： _[!UICONTROL Product Listing Actions]_未設定為 `Automatically list new products`。 | [[!UICONTROL Ready to List]](./ready-to-list.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md) | （成批操作）用於手動結束和刪除您的產品在Amazon上的清單。 只要已結束的清單符合您的上市規則資格，就可以重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md) | （成批活動）人工編輯現有的「改寫」，該改寫設定單個清單的價格、處理時間、條件和賣家附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Overrides]](./overrides.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Override]](./creating-editing-overrides.md) | 手動建立「覆蓋」，該「覆蓋」設定單個清單的價格、處理時間、條件和銷售者備注文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md) | 如果必須修改與目錄產品匹配的ASIN，則使用(例如：如果產品與錯誤的清單ASIN匹配)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md) | 可以提供兩個功能：<br><br>可用於在目錄產品和兩個Amazon清單之間建立1-2關係。 示例：Amazon的產品列有不同的ASIN值。 您可以將一個目錄產品與產品的兩個ASIN清單匹配。<br><br>可用於控制不同Amazon地區的清單。 示例：您有一個目錄產品，其中根據Amazon地區定義了不同的發運方法（美國地區為FBA，加拿大地區為FBM）。 要控制庫存/數量，您可以建立別名銷售商SKU，並在該區域中重新列出具有不同銷售商SKU的相同產品。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md)<br>[[!UICONTROL Ended]](./ended-listings.md) |
| [[!UICONTROL Switch to Fulfilled by Amazon/Merchant]](./fulfilled-by.md#configure-fulfilled-by-settings) | 用於修改與您的產品關聯的履行方法(由Amazon履行：FBA或由商家履行：FBM)。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL End Listing]](./end-listings-manually.md) | （單個清單操作）用於手動結束和刪除您的產品在Amazon上存在的清單。 只要已結束的清單符合您的上市規則資格，就可以重新列出。 | [[!UICONTROL Inactive]](./inactive-listings.md)<br>[[!UICONTROL Active]](./active-listings.md)<br>[[!UICONTROL Ineligible]](./ineligible-listings.md) |
| [[!UICONTROL Edit Override]](./creating-editing-overrides.md) | （單個清單操作）手動編輯現有的「改寫」，該「改寫」設定單個清單的價格、處理時間、條件和賣家附註文本，忽略其他清單預設值、設定和規則。 | [[!UICONTROL Overrides]](./overrides.md) |

## 訪問產品清單

1. 在 _管理_ 邊欄，轉到 **營銷** > _頻道_ > **AmazonSales Channel**。

1. 按一下 **查看儲存** 在商店卡上。

1. 在儲存儀表板上，按一下 **管理清單** 的 _儲存清單_ 的子菜單。
