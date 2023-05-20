---
title: 第三方清單
description: 更新第三方清單設定，確定您的Commerce目錄是否從您現有的Amazon銷售中心清單中導入產品。
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# 第三方清單

第三方清單設定是您的商店清單設定的一部分。 從 [儲存儀表板](./amazon-store-dashboard.md)。

這些設定確定 [!DNL Commerce] 將產品導入現有產品 [!DNL Amazon Seller Central] 清單。 最好從Amazon導入清單，以確保所有清單都匹配 [!DNL Commerce] 產品。 當您的清單是您的 [!DNL Commerce] 目錄，您可以從單個目錄管理您的所有產品，並使用Amazon銷售渠道功能。 這些功能包括與Amazon的履行和訂單管理，智慧重新定價和數量管理。

配置為導入您的Amazon清單時，Amazon銷售渠道會將您的Amazon清單導入您的 [!DNL Commerce] 目錄，嘗試將它們與現有產品匹配。 如果未自動找到匹配項，則可以將Amazon清單作為新清單導入 [!DNL Commerce] 產品或手動將清單與產品匹配。

如果您選擇導入Amazon清單，請選擇 [!DNL Commerce] 值的屬性。 如果你沒有 [!DNL Commerce] [產品屬性](./ob-creating-magento-attributes.md)，請考慮建立和分配它們。 映射這些屬性有助於將導入的Amazon清單與 [!DNL Commerce] 產品。

初始清單導入在 [儲存整合](./store-integration.md) 完成。 之後，根據你的密碼設定， [!DNL Commerce] 持續檢查新添加的Amazon清單(未在AmazonSales Channel中建立)並更新您的 [!DNL Commerce] 根據第三方清單設定編錄。

## 配置第三方清單設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店儀表板上。

1. 展開 _[!UICONTROL Third Party Listings]_的子菜單。

1. 對於 **[!UICONTROL Import Third Party Listings]** （必需），選擇選項：

   - `Import Listing`  — （預設）選擇何時希望從您的Amazon清單導入產品資訊 [!DNL Commerce] 產品目錄。 此選項是預設選項，建議使用。

   - `Do Not Import Listing`  — 選擇要手動執行的時間 [建立和分配新產品](https://docs.magento.com/user-guide/catalog/products.html){target="_blank"} 到 [!DNL Commerce] 你的Amazon清單目錄。
   >[!NOTE]
   >以下選項欄位僅在設定為時處於活動狀態 `Import Listing`。

1. 對於 **[!UICONTROL Attribute That Contains Amazon Seller SKU]**&#x200B;的子菜單。 [!DNL Commerce] 與Amazon賣家SKU值匹配的屬性。

1. 對於 **[!UICONTROL Attribute That Contains Amazon ASIN]**&#x200B;的子菜單。 [!DNL Commerce] 屬性，並將其與AmazonASIN匹配。

   >[!NOTE]
   >如果您沒有建立這些 [!DNL Commerce] 您的Amazon清單的屬性，請參閱 [為Amazon匹配建立屬性](./ob-creating-magento-attributes.md)。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**。

![第三方清單](assets/amazon-third-party-listings.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Import Third Party Listings] | 必需。 選項：<ul><li>**[!UICONTROL Import Listing]**  — （預設）選擇何時希望從您的Amazon清單導入產品資訊 [!DNL Commerce] 產品目錄。 </li><li>**[!UICONTROL Do Not Import Listing]**  — 選擇要手動執行的時間 [建立和分配新產品](https://docs.magento.com/user-guide/catalog/products.html){target="_blank"} 到 [!DNL Commerce] 你的Amazon清單目錄。</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | 僅在設定為時處於活動狀態 `Import Listing`。<br>選擇 [!DNL Commerce] 屬性，與Amazon賣家SKU的Amazon屬性匹配。 如果此屬性不存在，請參見 [為Amazon匹配建立Amazon產品屬性](./ob-creating-magento-attributes.md)。 如果需要，請查看 [!DNL Commerce] [屬性](./managing-attributes.md) 並建立或編輯與此Amazon資料匹配的屬性。 |
| [!UICONTROL Attribute That Contains Amazon ASIN] | 僅在設定為時處於活動狀態 `Import Listing`。<br>選擇 [!DNL Commerce] 與AmazonASIN的Amazon屬性匹配的屬性。 如果此屬性不存在，請參見 [為Amazon匹配建立Amazon產品屬性](./ob-creating-magento-attributes.md)。 如果需要，請查看 [!DNL Commerce] [屬性](./managing-attributes.md) 並建立或編輯與此Amazon資料匹配的屬性。 |

**快速訪問** - [!UICONTROL Listing Settings] 節

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
