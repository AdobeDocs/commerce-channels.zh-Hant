---
title: 第三方清單
description: 更新第三方清單設定，以判斷您的商務目錄是否從您現有的Amazon賣方中心清單匯入產品。
redirect_from: /sales-channels/asc/ob-third-party-listings.html
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 第三方清單

協力廠商清單設定是您商店清單設定的一部分。 清單設定可從[儲存控制面板](./amazon-store-dashboard.md)存取。

這些設定可確定您的[!DNL Commerce]目錄是否從現有的[!DNL Amazon Seller Central]清單匯入產品。 最佳實務是從Amazon匯入清單，以確保所有清單都有相符的[!DNL Commerce]產品。 當您的清單屬於[!DNL Commerce]目錄的一部分時，您可以從單一目錄管理所有產品，並使用Amazon銷售渠道功能。 這些功能包括使用Amazon完成和訂單管理、智慧重新定價和數量管理。

設定為匯入Amazon清單時，Amazon銷售管道會將您的Amazon清單匯入[!DNL Commerce]目錄，嘗試將它們與現有產品相符。 如果找不到相符項目，您可以將Amazon清單匯入為新[!DNL Commerce]產品，或手動將清單與產品比對。

如果您選擇匯入Amazon清單，請選擇具有Amazon賣家SKU和Amazon ASIN值的[!DNL Commerce]屬性。 如果您沒有[!DNL Commerce] [產品屬性](./ob-creating-magento-attributes.md)，請考慮建立並指派它們。 對應這些屬性有助於將匯入的Amazon清單正確比對至您的[!DNL Commerce]產品。

完成[store integration](./store-integration.md)後，初始清單匯入會起始。 之後並根據您的cron設定， [!DNL Commerce]會持續檢查是否有新增的Amazon清單(未在AmazonSales Channel中建立)，並根據您的第三方清單設定來更新您的[!DNL Commerce]目錄。

## 配置第三方清單設定

1. 按一下儲存控制面板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Third Party Listings]_區段。

1. 對於&#x200B;**[!UICONTROL Import Third Party Listings]**（必要），選擇一個選項：

   - `Import Listing`  — （預設）選擇何時要從Amazon清單中匯入產品資訊至 [!DNL Commerce] 產品目錄。此選項為預設值，建議使用。

   - `Do Not Import Listing`  — 選擇您想要手動建 [立新產品的時間](https://docs.magento.com/user-guide/catalog/products.html){:target=&quot;_blank&quot;}，並指派給您Amazon [!DNL Commerce] 清單的目錄。
   >[!NOTE]
   >下列選項欄位僅在設為`Import Listing`時有效。

1. 對於&#x200B;**[!UICONTROL Attribute That Contains Amazon Seller SKU]**，選擇與Amazon賣家SKU值相符的[!DNL Commerce]屬性。

1. 對於&#x200B;**[!UICONTROL Attribute That Contains Amazon ASIN]**，選擇您建立的[!DNL Commerce]屬性，並將其與Amazon ASIN匹配。

   >[!NOTE]
   >如果您未為Amazon清單建立這些[!DNL Commerce]屬性，請參閱[建立Amazon比對的屬性](./ob-creating-magento-attributes.md)。

1. 完成後，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![第三方清單](assets/amazon-third-party-listings.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Import Third Party Listings] | 必填。 選項：<ul><li>**[!UICONTROL Import Listing]**  — （預設）選擇何時要從Amazon清單中匯入產品資訊至 [!DNL Commerce] 產品目錄。 </li><li>**[!UICONTROL Do Not Import Listing]**  — 選擇您想要手動建 [立新產品的時間](https://docs.magento.com/user-guide/catalog/products.html){:target=&quot;_blank&quot;}，並指派給您Amazon [!DNL Commerce] 清單的目錄。</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | 僅在設為`Import Listing`時處於活動狀態。<br>選擇 [!DNL Commerce] 屬性，以比對Amazon賣家SKU的Amazon屬性。如果此屬性不存在，請參閱[建立Amazon產品屬性以供Amazon比對](./ob-creating-magento-attributes.md)。 如有需要，請查看[!DNL Commerce] [attributes](./managing-attributes.md)並建立或編輯屬性以符合此Amazon資料。 |
| [!UICONTROL Attribute That Contains Amazon ASIN] | 僅在設為`Import Listing`時處於活動狀態。<br>選擇 [!DNL Commerce] 與Amazon ASIN的Amazon屬性相符的屬性。如果此屬性不存在，請參閱[建立Amazon產品屬性以供Amazon比對](./ob-creating-magento-attributes.md)。 如有需要，請查看[!DNL Commerce] [attributes](./managing-attributes.md)並建立或編輯屬性以符合此Amazon資料。 |

**快速存取**  — 區 [!UICONTROL Listing Settings] 段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
