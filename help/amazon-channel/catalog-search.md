---
title: 目錄搜尋
description: 若要設定屬性比對，以協助將符合條件的商務目錄產品與Amazon清單對應，請更新目錄搜尋設定。
redirect_from: /sales-channels/asc/ob-catalog-search.html
exl-id: 9fcaa924-cba3-498f-8e21-1a1f91b1ad04
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '981'
ht-degree: 0%

---

# 目錄搜尋

_目錄_ 搜尋設定是您商店清單設定的一部分。清單設定可從[儲存控制面板](./amazon-store-dashboard.md)存取。

這些設定可讓您設定屬性比對，協助將符合條件的[!DNL Commerce]產品與Amazon清單對應。 映射後，Amazon將激活與定價、數量、改寫、訂單和產品同步相關的操作。

定義這些對應值會增加完全相符的可能性，將手動比對產品清單的需求減到最少。 將屬性新增為[預先設定任務](./amazon-pre-setup-tasks.md)的一部分，Amazon銷售管道在Amazon和[!DNL Commerce]之間上線及同步產品資料期間，更有可能自動比對您的產品。

如果您僅建立Amazon ASIN屬性（未為每個產品新增ASIN值），您的[!DNL Commerce]產品可能不會自動符合您的Amazon清單。 您可以[手動指派](./creating-assigning-catalog-products.md)您的產品。 不過，手動比對不會建立共用及同步產品資料所需的資料元素。

>[!IMPORTANT]
>
>如果您手動匹配產品，並且想要更新產品的ASIN、UPC或其他資料元素，則必須在兩個位置更新資料。 在[!DNL Commerce]目錄和[!DNL Amazon Seller Central]帳戶的Amazon清單中更新它。

最佳作法是對應這些屬性和值（若有）。 完成此對應並非必要項目，但有利於產品比對，且必須在Amazon和[!DNL Commerce]之間正確進行目錄同步。

如果要新增屬性，請參閱[建立Amazon比對的產品屬性](./ob-creating-magento-attributes.md)。

## 配置[!UICONTROL Catalog Search]設定

1. 按一下儲存控制面板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Catalog Search]_區段。

1. 對於&#x200B;**[!UICONTROL ASIN]**，選擇您為Amazon ASIN值建立的產品屬性。

   ASIN([!DNL Amazon Standard Identification Number])是由十個字母和/或數字組成的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。

1. 對於&#x200B;**[!UICONTROL EAN]**，選擇您為Amazon EAN值建立的產品屬性。

   歐洲商品編號(EAN)是條碼標準，是12碼或13碼的產品識別碼。 每個EAN都唯一標識產品、製造商及其屬性；通常，EAN將打印在產品標籤或包裝上，作為條碼。 Amazon需要EAN代碼來改善搜尋結果的品質和目錄的品質。 您可以從製造商處獲得EAN。

1. 對於&#x200B;**[!UICONTROL GCID]**，選擇為Amazon GCIN值建立的產品屬性。

   全域目錄識別碼(GCID)是沒有UPC程式碼或ISBN之產品的ID。 Amazon的Brand Registry可讓您註冊為品牌擁有者，並為產品建立唯一ID。

1. 對於&#x200B;**[!UICONTROL ISBN]**，選擇您為Amazon ISBN值建立的產品屬性。

   國際標準書號(ISBN)是唯一的商業圖書標識條碼。 每個ISBN代碼都唯一地標識一本書。 ISBN的位數為10或13。 2007年1月1日之後分配的所有ISBN都有13位數。

1. 對於&#x200B;**[!UICONTROL UPC]**，選擇您為Amazon UPC值建立的產品屬性。

   通用產品代碼(UPC)是12位數的條形碼，在美國廣泛用於零售包裝。

1. 對於&#x200B;**[!UICONTROL General Search]**，選擇要用於常規搜索匹配的產品屬性。

   此屬性是您可以選取，將[!DNL Commerce]產品與適當的Amazon清單相符。 一般搜尋會使用目錄中的關鍵字搜尋。 因此，建議使用[!DNL Commerce]屬性來包含相關關鍵字，例如產品SKU或產品名稱。 一般搜尋可能會傳回許多可能的相符項目，在這種情況下，您可以從可能的相符項目中選取適當的Amazon清單。 此欄位的常見選項為`Product Name`。

1. 完成後，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![目錄搜尋](assets/amazon-catalog-search.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL ASIN] | 10個字母和/或數字的唯一區塊，用於識別項目。<br><br>ASIN代表 [!DNL Amazon Standard Identification Number]。ASIN是10個字母和/或數字的唯一塊，用於標識項目。 對於帳簿，ASIN與ISBN號相同，但是對於所有其他產品，當項目上載到其目錄時將建立新的ASIN。 您可以在Amazon的產品詳細資訊頁面上找到項目ASIN，以及與項目相關的詳細資訊。 |
| [!UICONTROL EAN (European Article Number)] | 12位或13位的產品識別碼。 歐洲商品編號(EAN)是條碼標準，是12碼或13碼的產品識別碼。 每個EAN都唯一標識產品、製造商及其屬性；通常，EAN將打印在產品標籤或包裝上，作為條碼。 Amazon需要EAN代碼來改善搜尋結果的品質和目錄的品質。 您可以從製造商處獲得EAN。 |
| [!UICONTROL GCID (Global Catalog Identifier)] | 全域目錄識別碼(GCID)是沒有UPC程式碼或ISBN之產品的ID。 Amazon的Brand Registry可讓您註冊為品牌擁有者，並為可能沒有UPC或ISBN的產品建立唯一ID。 |
| [!UICONTROL ISBN (International Standard Book Number)] | 10位或13位的唯一商用圖書標識條碼。 國際標準書號(ISBN)是唯一的商業圖書標識條碼。 每個ISBN代碼都唯一地標識一本書。 ISBN的位數為10或13。 2007年1月1日之後分配的所有ISBN都有13位數。 |
| UPC（通用產品代碼） | 12位長條碼。 通用產品代碼(UPC)是12位數的條形碼，在美國廣泛用於零售包裝。 |
| [!UICONTROL General Search] | 選取屬性。 此屬性是您可以選取，將[!DNL Commerce]產品與適當的Amazon清單相符。 一般搜尋會使用目錄中的關鍵字搜尋。 因此，建議使用[!DNL Commerce]屬性來包含相關關鍵字，例如產品SKU或產品名稱。 一般搜尋可能會傳回許多可能的相符項目，在這種情況下，您可以從可能的相符項目中選取適當的Amazon清單。 此欄位的常見選項為`Product Name`。 |

**快速存取**  — 區 [!UICONTROL Listing Settings] 段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
