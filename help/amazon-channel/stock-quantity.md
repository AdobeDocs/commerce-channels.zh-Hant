---
title: 庫存/數量
description: 要控制產品數量詳細資訊從您的商務商店同步到您的 [!DNL Amazon Seller Central] 帳戶，更新「庫存/數量」設定。
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 庫存/數量

*[!UICONTROL Stock/Quantity]* 設定是您商店清單設定的一部分。 清單設定可從 [儲存儀表板](./amazon-store-dashboard.md).

這些設定可用來同步來自您 [!DNL Commerce] 店面數量 [!DNL Amazon Seller Central] 帳戶。 此工具功能強大，可向購買者顯示緊急狀況，同時讓詳細目錄保持井然有序，以用於其他廣告。 例如，某些商戶的倉庫中可能有150件特定SKU的物料，並想要確定Amazon購物者可以購買其所有庫存。 其他商家可能希望一次只列出一個項目，以給最終用戶造成一種稀缺感。 在此情況下，請設定 *[!UICONTROL Maximum Listed Quantity]* to `1`.

數量是地區屬性，並以 **[!UICONTROL Amazon Marketplace Country]** 設定期間定義 [商店整合](./store-integration.md). 產品數量變更時，此變更會影響共用該產品的所有Amazon清單 [!DNL Amazon Seller SKU] 在Amazon的商店裡賣的。 對共用的變更 [!DNL Amazon Seller SKU] 在美國，不會影響您為不同國家/地區設定的Amazon商店。 已整合的第一個Amazon商店（具有最舊的建立日期）會控制數量設定中的優先順序。

>[!NOTE]
>
>對於Adobe Commerce和Magento Open Source2.3.x使用者，Amazon銷售管道支援使用庫存管理擴充功能，不需進行任何額外設定。 請參閱 [管理庫存](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target=&quot;_blank&quot;}。

## 配置庫存/數量設定 {#configure-stock--quantity-settings}

1. 按一下 **[!UICONTROL Listing Settings]** 在商店控制面板上。

1. 展開 **[!UICONTROL Stock / Quantity]** 區段。

1. 針對 **[!UICONTROL Out-of-Stock Threshold]** （必要），輸入產品最少數量的數值，以使產品符合其Amazon清單的資格。

   預設為 `0`. 若您的 [!DNL Commerce] 產品庫存低於此數字，因此個別的Amazon清單不符合透過Amazon進行銷售的資格。

1. 針對 **[!UICONTROL Maximum Listed Quantity]** （必要），輸入您要在Amazon清單中顯示的數量的數值。

   此設定會以輸入的值列出所有符合資格的Amazon清單。 銷售項目時，Amazon列出數量不會變更。 即使您的實際產品數量高於或低於此值，可用清單數量仍始終使用此值。 當您不管理產品詳細目錄時，通常會使用此設定。 例如，您的 [!DNL Commerce] 目錄。 設為 `10`,Amazon清單一律會顯示可用數量 `10` 不會變更產品進行銷售的時機。

1. 針對 **[!UICONTROL "Do Not Manage Stock" Quantity]** （必要），輸入要為Amazon清單顯示的數量值。

   Amazon要求您發佈可用數量。 針對 [!DNL Commerce] 設為不管理庫存但您想將其列在Amazon的產品，則會發佈此清單，並在此處輸入可用數量。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**.

![庫存/數量設定](assets/amazon-stock-quantity.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | 輸入產品最少數量的數值，以使產品符合其Amazon清單的條件(預設為 `0`)。<br><br>若您的 [!DNL Commerce] 產品庫存低於此數字，因此個別的Amazon清單不符合透過Amazon進行銷售的資格。 |
| [!UICONTROL Maximum Listed Quantity] | 輸入要在Amazon清單中顯示的數量的數值。<br><br>銷售物料時，Amazon清單會重新發佈此處輸入的數量。 當您不管理產品詳細目錄時，通常會使用此設定。<br><br>例如，您可以將「列出的數量上限」值輸入為 `10`. 產品的實際數量為 `80`. 因為您已將此值設為 `10`,Amazon清單一律會顯示可用數量 `10`. 即使庫存量較低，可用數量仍始終以定義的值顯示。 |
| [!UICONTROL "Do Not Manage Stock" Quantity] | 為Amazon清單的顯示數量輸入值。<br><br>Amazon要求您發佈可用數量。 針對 [!DNL Commerce] 設為「不管理庫存」但您想將其列在Amazon的產品，則會發佈清單，並提供此處輸入值的可用數量。 |

**快速存取** - [!UICONTROL Listing Settings] 區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## 範例：最大列出數量

銷售物料時，Amazon清單會依此數量重新列出。

例如，若您設定 *[!UICONTROL Maximum Listed Quantity]* as `12`，即使產品有 [!DNL Commerce] 數量80:

![最大列出數量實例1](assets/amazon-max-listed-quantity.png)

如果您將 *[!UICONTROL Maximum Listed Quantity]* as `1`，則會列出所有合格產品，且數量 `1`. 當項目售出時，系統會尋找您的 [!DNL Commerce] 產品，若存在額外存貨，請以數量重新啟用Amazon上的項目 `1`.

此選項對於通常訂購量為1的產品可能很有價值。 此外，檢視Amazon清單時，也會增加購物者的迫切性。

![最大列出數量實例2](assets/amazon-max-listed-quantity-1.png)
