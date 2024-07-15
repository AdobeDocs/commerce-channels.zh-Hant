---
title: AmazonSales Channel- [!UICONTROL Third-party Listings]
description: 更新協力廠商清單設定可判斷您的Commerce目錄是否從您現有的Amazon賣家中心清單匯入產品。
feature: Sales Channels, Products
exl-id: bc82775a-6f29-49b5-a80b-20e171eaf8f4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# [!UICONTROL Third-party Listings]

協力廠商清單設定是商店清單設定的一部分。 清單設定可從[存放區儀表板](./amazon-store-dashboard.md)存取。

這些設定決定您的[!DNL Commerce]目錄是否從您現有的[!DNL Amazon Seller Central]清單匯入產品。 最佳實務是從Amazon匯入清單，以確保所有清單都具有相符的[!DNL Commerce]產品。 當您的清單是[!DNL Commerce]目錄的一部分時，您可以從單一目錄管理您的所有產品，並使用Amazon銷售管道功能。 這些功能包括使用Amazon進行履行與訂單管理、智慧型重新訂價，以及數量管理。

當設定為匯入您的Amazon清單時，Amazon銷售管道會將您的Amazon清單匯入您的[!DNL Commerce]目錄，嘗試比對它們與現有的產品。 如果未自動找到相符專案，您可以將Amazon清單匯入為新的[!DNL Commerce]產品，或手動比對清單與產品。

如果您選擇匯入Amazon清單，請選擇具有Amazon賣家SKU和Amazon ASIN值的[!DNL Commerce]屬性。 如果您沒有[!DNL Commerce] [產品屬性](./ob-creating-magento-attributes.md)，請考慮建立並指派這些屬性。 對應這些屬性有助於正確比對匯入的Amazon清單與您的[!DNL Commerce]產品。

當[存放區整合](./store-integration.md)完成時，初始清單匯入會啟動。 之後，根據您的cron設定，[!DNL Commerce]會持續檢查新新增的Amazon清單(不是在AmazonSales Channel中建立的)，並根據您的協力廠商清單設定更新您的[!DNL Commerce]目錄。

## 設定協力廠商清單設定

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Third Party Listings]_區段。

1. 針對&#x200B;**[!UICONTROL Import Third Party Listings]** （必要），請選擇選項：

   - `Import Listing` - （預設）選擇您希望Amazon清單中的產品資訊匯入[!DNL Commerce]產品目錄的時間。 此選項為預設值，建議使用。

   - `Do Not Import Listing` — 選擇何時要手動[建立新產品](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html)並指派給您的Amazon清單的[!DNL Commerce]目錄。

   >[!NOTE]
   >下列選項欄位只有在設定為`Import Listing`時才有效。

1. 針對&#x200B;**[!UICONTROL Attribute That Contains Amazon Seller SKU]**，選擇與Amazon賣家SKU值相符的[!DNL Commerce]屬性。

1. 針對&#x200B;**[!UICONTROL Attribute That Contains Amazon ASIN]**，選擇您建立的[!DNL Commerce]屬性，並將其與Amazon ASIN比對。

   >[!NOTE]
   >如果您沒有為Amazon清單建立這些[!DNL Commerce]屬性，請參閱[為Amazon比對建立屬性](./ob-creating-magento-attributes.md)。

1. 完成時，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![協力廠商清單](assets/amazon-third-party-listings.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Import Third Party Listings] | 必填。 選項：<ul><li>**[!UICONTROL Import Listing]** - （預設）選擇您希望Amazon清單中的產品資訊匯入[!DNL Commerce]產品目錄的時間。 </li><li>**[!UICONTROL Do Not Import Listing]** — 選擇何時要手動[建立新產品](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html)並指派給您的Amazon清單的[!DNL Commerce]目錄。</li></ul> |
| [!UICONTROL Attribute That Contains Amazon Seller SKU] | 僅在設定為`Import Listing`時啟用。<br>選擇[!DNL Commerce]屬性，做為與Amazon賣家SKU之Amazon屬性的相符專案。 如果此屬性不存在，請參閱[為Amazon比對建立Amazon產品屬性](./ob-creating-magento-attributes.md)。 如有需要，請檢閱您的[!DNL Commerce] [屬性](./managing-attributes.md)，並建立或編輯屬性以符合此Amazon資料。 |
| [!UICONTROL Attribute That Contains Amazon ASIN] | 僅在設定為`Import Listing`時啟用。<br>選擇與Amazon ASIN的Amazon屬性相符的[!DNL Commerce]屬性。 如果此屬性不存在，請參閱[為Amazon比對建立Amazon產品屬性](./ob-creating-magento-attributes.md)。 如有需要，請檢閱您的[!DNL Commerce] [屬性](./managing-attributes.md)，並建立或編輯屬性以符合此Amazon資料。 |

**快速存取** - [!UICONTROL Listing Settings]區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
