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

_[!UICONTROL Product Listings]_頁面包含數個索引標籤，您可從這些索引標籤檢視所有清單的狀態，並將您的產品與Amazon清單比對。

可用的清單工作在每個索引標籤上稍有不同，但[工作區控制項](./workspace-controls.md)相同，可讓您自訂清單顯示的資料。

**[!UICONTROL Actions]**&#x200B;下的選項可以將動作套用至多個清單，而&#x200B;_[!UICONTROL Action]_欄中&#x200B;**[!UICONTROL Select]**下的選項僅會將動作套用至個別清單。

另請參閱[依動作管理清單](./managing-listings-by-action.md)。

![產品清單標籤](assets/amazon-product-listings-tabs.png){width="600" zoomable="yes"}

| 標籤 | 說明 | 動作 |
|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Incomplete]](./incomplete-listings.md) | 顯示您的[!DNL Commerce]目錄產品，這些產品符合您定義的清單設定，但遺失Amazon的清單所需資訊。<br><br>如果在您的[_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md)設定中將&#x200B;_[!UICONTROL Automatic List Action]_設定為`Automatically List Eligible Products`，這些專案就是您的&#x200B;**[!UICONTROL In Progress Listings]**。 | [!UICONTROL Reattempt auto match to Amazon Listing]<br>[[!UICONTROL Update Required Info]](./amazon-manually-update-incomplete-listing.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL New Third Party]](./new-third-party-listings.md) | 顯示與您[!DNL Commerce]目錄中的產品不符的現有Amazon清單(根據從Amazon收到的資訊)。 | [[!UICONTROL Create New Catalog Product(s)]](./creating-assigning-catalog-products.md)<br>嘗試自動比對<br>[[!UICONTROL Assign Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL Create New Catalog Product]](./creating-assigning-catalog-products.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ready to List]](./ready-to-list.md) | 顯示已準備好建立Amazon清單的目錄產品，但您的商店設定為不會自動發佈新清單。 此索引標籤可用來手動發佈您的新清單。<br><br>如果在您的[_[!UICONTROL Product Listing Actions]_](./product-listing-actions.md)設定中將&#x200B;_[!UICONTROL Automatic List Action]_設定為`Do Not Automatically List Eligible Products`，這些專案就是您的&#x200B;**[!UICONTROL In Progress Listings]**。 | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Inactive]](./inactive-listings.md) | 顯示已發佈至Amazon的目錄產品，但Amazon尚未核准此清單的「作用中」狀態。 | 在Amazon](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換到由Amazon/商家履行的[結束清單<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Active]](./active-listings.md) | 顯示您的Amazon清單，這些清單已與您[!DNL Commerce]目錄中的產品相符、已發佈至Amazon，且已由Amazon設定為作用中狀態。 | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換為由Amazon/商家履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Overrides]](./overrides.md) | 顯示符合已定義覆寫條件且已套用覆寫的Amazon清單。 覆寫優先於任何其他帳戶設定。 | [[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md) |
| [[!UICONTROL Ineligible]](./ineligible-listings.md) | 根據您定義的[清單設定](./listing-settings.md)，顯示您現有的Amazon清單，這些清單已不再適用。 | [[!UICONTROL End Listing(s) on Amazon]](./end-listings-manually.md)<br>[[!UICONTROL Edit Listing Overrides]](./creating-editing-overrides.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Create Override]](./creating-editing-overrides.md)<br>[[!UICONTROL Edit Assigned ASIN]](./edit-assigned-asin.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific)<br>切換為由Amazon/商家履行<br>[[!UICONTROL End Listing]](./end-listings-manually.md) |
| [[!UICONTROL Ended]](./ended-listings.md) | 顯示您已從Amazon手動結束（移除）的Amazon清單。 | [[!UICONTROL Publish Product to Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL View Details]](./product-listing-details.md)<br>[[!UICONTROL Publish On Amazon]](./publish-listings-manually.md)<br>[[!UICONTROL Create Alias Seller SKU]](./create-alias-seller-sku.md#region-specific) |

## 存取產品清單

1. 在&#x200B;_管理員_&#x200B;側邊欄上，移至&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下商店資訊卡上的&#x200B;**[!UICONTROL View Store]**。

1. 在存放區儀表板上，按一下&#x200B;_[!UICONTROL Store Listings]_區段中的&#x200B;**[!UICONTROL Manage Listings]**。
