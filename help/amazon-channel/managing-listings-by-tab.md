---
title: 按狀態/頁簽管理產品清單
description: 當您管理Amazon清單時，可以根據狀態將動作套用至清單。
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 按狀態/頁簽管理產品清單

此 _[!UICONTROL Product Listings]_頁面包含數個標籤，您可從中檢視所有清單的狀態，並將產品與Amazon清單配對。

每個標籤上可用的清單任務稍有不同，但 [工作區控制項](./workspace-controls.md) 相同，可讓您自訂為清單顯示的資料。

下方的選項 **[!UICONTROL Actions]** 可將動作套用至多個清單，而 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄僅將動作套用至個別清單。

另請參閱 [按操作管理清單](./managing-listings-by-action.md).

![產品清單索引標籤](assets/amazon-product-listings-tabs.png)

| 標籤 | 說明 | 動作 |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | 顯示 [!DNL Commerce] 目錄產品符合您定義的清單設定，但缺少Amazon要求的清單資訊。<br><br>若 _[!UICONTROL Automatic List Action]_設為 `Automatically List Eligible Products` 在 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定，這些項目是&#x200B;**[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | 顯示與您的產品不符的現有Amazon清單(根據從Amazon收到的資訊) [!DNL Commerce] 目錄。 | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>嘗試自動匹配<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | 顯示已準備好建立Amazon清單的目錄產品，但您的商店設定為不會自動發佈新清單。 此索引標籤可用來手動發佈新清單。<br><br>若 _[!UICONTROL Automatic List Action]_設為 `Do Not Automatically List Eligible Products` 在 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定，這些項目是&#x200B;**[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | 顯示已發佈至Amazon，但Amazon尚未核准「作用中」狀態清單的目錄產品。 | [結束 Amazon上市](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換至由Amazon/Merchant履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | 顯示與您的 [!DNL Commerce] 目錄、已發佈至Amazon，且已由Amazon設為「作用中」狀態。 | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換至由Amazon/Merchant履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | 顯示符合已定義覆寫條件且已套用覆寫的Amazon清單。 優先順序高於任何其他帳戶設定。 | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | 根據您定義的，顯示不再符合資格的現有Amazon清單 [清單設定](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換至由Amazon/Merchant履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | 顯示已從Amazon手動結束（移除）的Amazon清單。 | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## 存取產品清單

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在商店控制面板上，按一下 **[!UICONTROL Manage Listings]** 在 _[!UICONTROL Store Listings]_區段。
