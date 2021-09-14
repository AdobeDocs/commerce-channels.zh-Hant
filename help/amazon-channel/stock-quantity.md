---
title: 庫存/數量
description: 要控制從您的Commerce商店到 [!DNL Amazon Seller Central] 帳戶的產品數量詳細資訊的同步，請更新「庫存/數量」設定。
redirect_from: /sales-channels/asc/ob-stock-quantity.html
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 庫存/數量

*[!UICONTROL Stock/Quantity]* 設定是您商店清單設定的一部分。清單設定可從[儲存控制面板](./amazon-store-dashboard.md)存取。

這些設定用於將產品數量詳細資訊從您的[!DNL Commerce]店面同步到您的[!DNL Amazon Seller Central]帳戶上的數量。 此工具功能強大，可向購買者顯示緊急狀況，同時讓詳細目錄保持井然有序，以用於其他廣告。 例如，某些商戶的倉庫中可能有150件特定SKU的物料，並想要確定Amazon購物者可以購買其所有庫存。 其他商家可能希望一次只列出一個項目，以給最終用戶造成一種稀缺感。 在此情況下，將&#x200B;*[!UICONTROL Maximum Listed Quantity]*&#x200B;設定為`1`。

數量是區域屬性，並根據[儲存整合](./store-integration.md)期間定義的&#x200B;**[!UICONTROL Amazon Marketplace Country]**&#x200B;設定。 對產品數量進行變更時，變更會影響在相同國家/地區銷售之Amazon商店中共用該[!DNL Amazon Seller SKU]的所有Amazon清單。 在美國對共用[!DNL Amazon Seller SKU]所做的變更不會影響您為不同國家/地區設定的Amazon商店。 已整合的第一個Amazon商店（具有最舊的建立日期）會控制數量設定中的優先順序。

>[!NOTE]
>
>對於Adobe商務和Magento Open Source2.3.x使用者，Amazon銷售管道支援使用庫存管理擴充功能，不需進行任何額外設定。 請參閱[管理清單](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){:target=&quot;_blank&quot;}。

## 配置庫存/數量設定 {#configure-stock--quantity-settings}

1. 按一下儲存控制面板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;**[!UICONTROL Stock / Quantity]**&#x200B;區段。

1. 對於&#x200B;**[!UICONTROL Out-of-Stock Threshold]**（必要），輸入產品最少數量的數值，以使產品符合其Amazon清單的資格。

   預設值為`0`。 如果您的[!DNL Commerce]產品庫存低於此數字，則個別Amazon清單不符合透過Amazon進行銷售的資格。

1. 對於&#x200B;**[!UICONTROL Maximum Listed Quantity]**（必要），輸入要在Amazon清單中顯示的數量的數值。

   此設定會以輸入的值列出所有符合資格的Amazon清單。 銷售項目時，Amazon列出數量不會變更。 即使您的實際產品數量高於或低於此值，可用清單數量仍始終使用此值。 當您不管理產品詳細目錄時，通常會使用此設定。 例如，您的[!DNL Commerce]目錄中可能有數量為80的產品。 設為`10`時，Amazon清單一律會顯示可用數量`10`，且在產品進行銷售時不會變更。

1. 對於&#x200B;**[!UICONTROL "Do Not Manage Stock" Quantity]**（必要），輸入要顯示Amazon清單的數量值。

   Amazon要求您發佈可用數量。 若[!DNL Commerce]產品設定為不管理庫存，但您想將其列在Amazon上，則會發佈此清單，並在此處輸入可用數量。

1. 完成後，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![庫存/數量設定](assets/amazon-stock-quantity.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Out-of-Stock Threshold] | 輸入產品最少數量的數值，以使產品符合其Amazon清單的條件（預設值為`0`）。<br><br>如果您 [!DNL Commerce] 的產品庫存低於此數字，則個別Amazon清單不符合透過Amazon進行銷售的資格。 |
| [!UICONTROL Maximum Listed Quantity] | 輸入要在Amazon清單中顯示的數量的數值。<br><br>銷售物料時，Amazon清單會重新發佈此處輸入的數量。當您不管理產品詳細目錄時，通常會使用此設定。<br><br>例如，您可以輸入「列出的數量上限」值 `10`。產品的實際數量為`80`。 由於您已將此值設為`10`，因此Amazon清單一律會顯示可用數量`10`。 即使庫存量較低，可用數量仍始終以定義的值顯示。 |
| [!UICONTROL "Do Not Manage Stock" Quantity] | 為Amazon清單的顯示數量輸入值。<br><br>Amazon要求您發佈可用數量。若[!DNL Commerce]產品設定為不管理庫存，但您想將其列在Amazon上，則會發佈此清單，其中包含此處輸入值的可用數量。 |

**快速存取**  — 區 [!UICONTROL Listing Settings] 段

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

例如，如果您將&#x200B;*[!UICONTROL Maximum Listed Quantity]*&#x200B;設為`12`，即使產品的[!DNL Commerce]數量為80,Amazon清單仍會顯示數量12:

![最大列出數量實例1](assets/amazon-max-listed-quantity.png)

如果您將&#x200B;*[!UICONTROL Maximum Listed Quantity]*&#x200B;設為`1`，則所有合格產品都會列出數量`1`。 銷售項目時，系統會查看您的[!DNL Commerce]產品，如果存在額外庫存，則會以`1`數量重新啟用Amazon上的項目。

此選項對於通常訂購量為1的產品可能很有價值。 此外，檢視Amazon清單時，也會增加購物者的迫切性。

![最大列出數量實例2](assets/amazon-max-listed-quantity-1.png)
