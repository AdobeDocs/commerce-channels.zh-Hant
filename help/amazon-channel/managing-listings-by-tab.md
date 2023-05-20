---
title: 按狀態/頁籤管理產品清單
description: 在管理Amazon清單時，可以根據狀態將操作應用於清單。
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 按狀態/頁籤管理產品清單

的 _[!UICONTROL Product Listings]_頁面包含多個頁籤，您可以從中查看所有清單的狀態，並將產品與Amazon清單匹配。

每個頁籤上可用的清單任務略有不同，但 [工作區控制項](./workspace-controls.md) 相同，允許您自定義為清單顯示的資料。

選項 **[!UICONTROL Actions]** 可以將操作應用於多個清單，同時 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_列將操作僅應用於單個清單。

另請參閱 [按操作管理清單](./managing-listings-by-action.md)。

![「產品清單」頁籤](assets/amazon-product-listings-tabs.png)

| 頁籤 | 說明 | 操作 |
|--- |--- |--- |
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | 顯示 [!DNL Commerce] 符合您定義的清單設定但缺少Amazon清單所需資訊的目錄產品。<br><br>如果 _[!UICONTROL Automatic List Action]_設定為 `Automatically List Eligible Products` 在 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定，這些項目是您&#x200B;**[!UICONTROL In Progress Listings]**。 | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | 顯示您現有的與您的產品不匹配的Amazon清單(基於從Amazon收到的資訊) [!DNL Commerce] 目錄。 | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>嘗試自動匹配<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | 顯示已準備好建立Amazon清單的目錄產品，但您的商店設定為不自動發佈新清單。 此頁籤用於手動發佈新清單。<br><br>如果 _[!UICONTROL Automatic List Action]_設定為 `Do Not Automatically List Eligible Products` 在 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定，這些項目是您&#x200B;**[!UICONTROL In Progress Listings]**。 | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | 顯示已發佈到Amazon的目錄產品，但Amazon尚未批准清單「有效」狀態。 | [結束 Amazon上市](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換到由Amazon/商家履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | 顯示與您的產品匹配的Amazon清單 [!DNL Commerce] 目錄、已發佈給Amazon，並由Amazon提供「主動」地位。 | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換到由Amazon/商家履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | 顯示符合已定義覆蓋條件且已應用覆蓋的Amazon清單。 替代優先於任何其他帳戶設定。 | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | 根據您定義的清單顯示您現有的不再符合條件的Amazon清單 [清單設定](./listing-settings.md)。 | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換到由Amazon/商家履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | 顯示已從Amazon手動結束（刪除）的Amazon清單。 | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## 訪問產品清單

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下 **[!UICONTROL View Store]** 在商店卡上。

1. 在儲存儀表板上，按一下 **[!UICONTROL Manage Listings]** 的 _[!UICONTROL Store Listings]_的子菜單。
