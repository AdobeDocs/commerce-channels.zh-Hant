---
title: 依狀態/標籤管理Amazon產品清單
description: 當您管理Amazon清單時，可以根據狀態將動作套用至清單。
feature: Sales Channels, Products
exl-id: 33effdd8-baa9-4fc5-8c7e-313175eb7e9c
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 依狀態/標籤管理Amazon產品清單

此 _[!UICONTROL Product Listings]_頁面包含數個索引標籤，您可在其中檢視所有清單的狀態，並將產品與Amazon清單比對。

每個標籤上的可用清單任務略有不同，但 [工作區控制項](./workspace-controls.md) 相同，並可讓您自訂要針對清單顯示的資料。

下的選項 **[!UICONTROL Actions]** 可以將動作套用至多個清單，而選項位於 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄只會將此動作套用至個別清單。

另請參閱 [依動作管理清單](./managing-listings-by-action.md).

![產品清單標籤](assets/amazon-product-listings-tabs.png){width="600" zoomable="yes"}

| 標籤 | 說明 | 動作 |
|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | 顯示您的 [!DNL Commerce] 符合您定義的清單設定，但缺少Amazon清單所需資訊的目錄產品。<br><br>如果 _[!UICONTROL Automatic List Action]_設為 `Automatically List Eligible Products` 在您的 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定，這些專案是您的&#x200B;**[!UICONTROL In Progress Listings]**. | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | 顯示您現有的Amazon清單(根據從Amazon收到的資訊)，這些清單不符合您網站上的產品 [!DNL Commerce] 目錄。 | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>嘗試自動比對<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | 顯示已準備好建立Amazon清單的目錄產品，但您的商店設定為不會自動發佈新清單。 此索引標籤可用來手動發佈您的新清單。<br><br>如果 _[!UICONTROL Automatic List Action]_設為 `Do Not Automatically List Eligible Products` 在您的 [_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md) 設定，這些專案是您的&#x200B;**[!UICONTROL In Progress Listings]**. | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | 顯示已發佈至Amazon的目錄產品，但Amazon尚未核准此清單的「作用中」狀態。 | [結束 Amazon上的清單](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換至「由Amazon/商家履行」<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | 顯示您的Amazon清單，這些清單已與貴組織中的產品相符 [!DNL Commerce] 目錄、已發佈至Amazon且已由Amazon設為作用中狀態。 | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換至「由Amazon/商家履行」<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | 顯示符合已定義覆寫條件且已套用覆寫的Amazon清單。 覆寫優先於任何其他帳戶設定。 | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | 根據您定義的內容，顯示已不符合資格的現有Amazon清單 [清單設定](./listing-settings.md). | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換至「由Amazon/商家履行」<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | 顯示您已從Amazon手動結束（移除）的Amazon清單。 | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## 存取產品清單

1. 在 _管理員_ 側欄，前往 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 按一下 **[!UICONTROL View Store]** 在商店資訊卡上。

1. 在商店控制面板上，按一下 **[!UICONTROL Manage Listings]** 在 _[!UICONTROL Store Listings]_區段。
