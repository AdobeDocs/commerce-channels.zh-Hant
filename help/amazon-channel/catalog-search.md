---
title: Amazon清單的目錄搜尋
description: 若要設定有助於將合格Commerce目錄產品與Amazon清單對應的屬性比對，請更新目錄搜尋設定。
feature: Sales Channels, Search, Catalog Management, Products, Configuration
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 8c72b7db5472a573bd8c26acafdf7a3400875477
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---

# Amazon清單的目錄搜尋

_目錄搜尋_&#x200B;設定是商店清單設定的一部分。 清單設定可從[存放區儀表板](./amazon-store-dashboard.md)存取。

這些設定可讓您設定屬性比對，協助將合格的[!DNL Commerce]產品與Amazon清單對應。 對應後，Amazon會啟動與定價、數量、覆寫以及訂單和產品同步化相關的動作。

定義這些對應值會增加完全相符的可能性，將手動比對產品清單的需求降到最低。 將屬性新增為[預先設定工作](./amazon-pre-setup-tasks.md)的一部分，Amazon銷售管道在產品上線期間自動比對產品的可能性較高，並且在Amazon和[!DNL Commerce]之間同步產品資料。

如果您只建立Amazon ASIN屬性（未新增每個產品的ASIN值），則您的[!DNL Commerce]產品可能不會自動符合您的Amazon清單。 您可以[手動指派](./creating-assigning-catalog-products.md)您的產品。 不過，手動比對不會建立共用和同步產品資料所需的資料元素。

>[!IMPORTANT]
>
>如果您手動比對產品，而且想要更新產品的ASIN、UPC或其他資料元素，則必須更新兩個位置的資料。 在您的[!DNL Commerce]目錄和[!DNL Amazon Seller Central]帳戶的Amazon清單中更新它。

如果可用，對應這些屬性和值是最佳作法。 完成此對應並非必要操作，但有利於產品比對，且在Amazon與[!DNL Commerce]之間需要正確的目錄同步。

若要新增屬性，請參閱[建立Amazon相符的產品屬性](./ob-creating-magento-attributes.md)。

## 設定[!UICONTROL Catalog Search]設定

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Catalog Search]_區段。

1. 針對&#x200B;**[!UICONTROL ASIN]**，選擇您為Amazon ASIN值建立的產品屬性。

   ASIN ([!DNL Amazon Standard Identification Number])是識別專案的10個字母和/或數字的唯一區塊。 對於書籍，ASIN與ISBN編號相同，但對於所有其他產品，當專案上傳到它們的目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資料頁面上找到專案ASIN，以及與此專案相關的其他詳細資料。

1. 針對&#x200B;**[!UICONTROL EAN]**，選擇您為Amazon EAN值建立的產品屬性。

   歐洲文章編號(EAN)是一種條碼標準，是12或13位數的產品識別碼。 每個EAN都可唯一識別產品、製造商及其屬性；通常EAN會列印在產品標籤或包裝上作為條碼。 Amazon需要EAN程式碼來改善搜尋結果的品質和目錄的品質。 您可以向製造商取得EAN。

1. 針對&#x200B;**[!UICONTROL GCID]**，選擇您為Amazon GCIN值建立的產品屬性。

   通用類別目錄識別碼(GCID)是沒有UPC程式碼或ISBN之產品的ID。 Amazon的Brand Registry可讓您註冊為品牌擁有者，並為產品建立唯一ID。

1. 針對&#x200B;**[!UICONTROL ISBN]**，選擇您為Amazon ISBN值建立的產品屬性。

   國際標準書號(ISBN)是一種唯一的商業書籍識別碼條碼。 每個ISBN程式碼都可唯一識別書冊。 ISBN有10或13位數。 在2007年1月1日之後指派的所有ISBN都有13位數。

1. 針對&#x200B;**[!UICONTROL UPC]**，選擇您為Amazon UPC值建立的產品屬性。

   通用產品代碼(UPC)是一種12位數的條碼，在美國廣泛用於零售包裝。

1. 針對&#x200B;**[!UICONTROL General Search]**，選擇您要用於一般搜尋比對的產品屬性。

   您可以選取這個屬性，以比對[!DNL Commerce]產品與適當的Amazon清單。 一般搜尋會使用您目錄中的關鍵字搜尋。 因此，建議使用包含相關關鍵字（例如產品SKU或產品名稱）的[!DNL Commerce]屬性。 一般搜尋可能會傳回許多可能的相符專案，在這種情況下，您可以從可能的相符專案中選擇適當的Amazon清單。 此欄位的一般選取專案是`Product Name`。

1. 完成時，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![目錄搜尋](assets/amazon-catalog-search.png){width="500" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL ASIN] | 識別專案的10個字母和/或數字的唯一區塊。<br><br>ASIN代表[!DNL Amazon Standard Identification Number]。 ASIN是識別專案的10個字母和/或數字的唯一區塊。 對於書籍，ASIN與ISBN編號相同，但對於所有其他產品，當專案上傳到它們的目錄時會建立新的ASIN。 您可以在Amazon的產品詳細資料頁面上找到專案ASIN，以及與此專案相關的其他詳細資料。 |
| [!UICONTROL EAN (European Article Number)] | 12或13位數的產品識別碼。 歐洲文章編號(EAN)是一種條碼標準，是12或13位數的產品識別碼。 每個EAN都可唯一識別產品、製造商及其屬性；通常EAN會列印在產品標籤或包裝上作為條碼。 Amazon需要EAN程式碼來改善搜尋結果的品質和目錄的品質。 您可以向製造商取得EAN。 |
| [!UICONTROL GCID (Global Catalog Identifier)] | 通用類別目錄識別碼(GCID)是沒有UPC程式碼或ISBN之產品的ID。 Amazon的品牌登入可讓您註冊為品牌擁有者，並為可能沒有UPC或ISBN的產品建立唯一ID。 |
| [!UICONTROL ISBN (International Standard Book Number)] | 10或13位數的唯一商業書籍識別碼條碼。 國際標準書號(ISBN)是一種唯一的商業書籍識別碼條碼。 每個ISBN程式碼都可唯一識別書冊。 ISBN有10或13位數。 在2007年1月1日之後指派的所有ISBN都有13位數。 |
| UPC （通用產品代碼） | 12位數的條碼。 通用產品代碼(UPC)是一種12位數的條碼，在美國廣泛用於零售包裝。 |
| [!UICONTROL General Search] | 選取屬性。 您可以選取這個屬性，以比對[!DNL Commerce]產品與適當的Amazon清單。 一般搜尋會使用您目錄中的關鍵字搜尋。 因此，建議使用包含相關關鍵字（例如產品SKU或產品名稱）的[!DNL Commerce]屬性。 一般搜尋可能會傳回許多可能的相符專案，在這種情況下，您可以從可能的相符專案中選擇適當的Amazon清單。 此欄位的一般選取專案是`Product Name`。 |

**快速存取** - [!UICONTROL Listing Settings]區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
