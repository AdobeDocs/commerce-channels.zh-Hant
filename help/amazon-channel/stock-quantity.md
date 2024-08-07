---
title: AmazonSales Channel- [!UICONTROL Stock/Quantity]
description: 若要控制將產品數量詳細資料從您的Commerce商店同步至您的 [!DNL Amazon Seller Central] 帳戶，請更新「庫存/數量」設定。
feature: Sales Channels, Inventory
exl-id: a8b7ab6c-393c-43c6-b5ef-68845177edff
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# [!UICONTROL Stock/Quantity]

*[!UICONTROL Stock/Quantity]*&#x200B;設定是商店清單設定的一部分。 清單設定可從[存放區儀表板](./amazon-store-dashboard.md)存取。

這些設定可用來將您[!DNL Commerce]店面的產品數量詳細資料同步至您[!DNL Amazon Seller Central]帳戶上的數量。 此工具功能強大，可讓買家看到緊迫感，同時妥善整理庫存，以便進行額外廣告。 例如，有些商戶的倉庫中可能有150件特定SKU的庫存，且想要確保Amazon購物者可以購買其所有庫存。 其他商戶可能希望一次只列出一個專案，讓一般使用者產生稀缺感。 在此情況下，請將&#x200B;*[!UICONTROL Maximum Listed Quantity]*&#x200B;設定為`1`。

數量是區域屬性，且以[存放區整合](./store-integration.md)期間定義的&#x200B;**[!UICONTROL Amazon Marketplace Country]**&#x200B;設定為基礎。 當對產品的數量進行變更時，該變更會影響在同一個國家/地區銷售的Amazon商店中共用該[!DNL Amazon Seller SKU]的所有Amazon清單。 變更在美國的共用[!DNL Amazon Seller SKU]不會影響您為其他國家/地區設定的Amazon商店。 您第一個整合的Amazon存放區（具有最舊的建立日期）會控制數量設定中的優先順序。

>[!NOTE]
>
>對於Adobe Commerce和Magento Open Source 2.3.x使用者，Amazon Sales Channel支援使用Inventory management擴充功能，無需任何其他設定。 請參閱[管理詳細目錄](https://docs.magento.com/user-guide/v2.3/catalog/inventory-management.html){target="_blank"}。

## 設定庫存/數量設定 {#configure-stock--quantity-settings}

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;**[!UICONTROL Stock / Quantity]**&#x200B;區段。

1. 針對&#x200B;**[!UICONTROL Out-of-Stock Threshold]** （必要），請輸入產品最低數量的數值，以保持產品符合其Amazon清單的資格。

   預設值為`0`。 如果您的[!DNL Commerce]產品庫存低於此數字，則個別Amazon清單不符合透過Amazon進行銷售的資格。

1. 針對&#x200B;**[!UICONTROL Maximum Listed Quantity]** （必要），請輸入您要在Amazon清單中顯示的數量數值。

   此設定會依輸入值列出所有符合條件的Amazon清單。 銷售料號時，Amazon的清單數量不會變更。 清單可用數量一律使用此值，即使實際產品數量高於或低於此值。 此設定通常用於不管理產品詳細目錄時。 例如，您的[!DNL Commerce]目錄中可能有數量為80的產品。 設定為`10`時，Amazon清單一律會顯示可用數量`10`，且在針對產品進行銷售時不會變更。

1. 針對&#x200B;**[!UICONTROL "Do Not Manage Stock" Quantity]** （必要），請輸入要針對您的Amazon清單顯示的數量值。

   Amazon會要求您發佈可用數量。 針對設定為不管理庫存但您想要在Amazon上列出的[!DNL Commerce]產品，此清單會以此處輸入的可用數量發佈。

1. 完成時，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![庫存/數量設定](assets/amazon-stock-quantity.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Out-of-Stock Threshold] | 輸入產品最低數量的數值，以保持產品符合其Amazon清單的資格（預設為`0`）。<br><br>如果您的[!DNL Commerce]產品庫存低於此數字，則個別Amazon清單不符合透過Amazon銷售的資格。 |
| [!UICONTROL Maximum Listed Quantity] | 輸入您要在Amazon清單中顯示的數量數值。<br><br>銷售料號時，Amazon清單會以此處輸入的數量重新發佈。 此設定通常用於不管理產品詳細目錄時。<br><br>例如，您輸入的「列出數量上限」值為`10`。 您產品的實際數量為`80`。 因為您已將此值設定為`10`，Amazon清單一律會顯示`10`的可用數量。 可用數量一律以定義的值顯示，即使存貨數量較低。 |
| [!UICONTROL "Do Not Manage Stock" Quantity] | 輸入Amazon清單的顯示數量值。<br><br>Amazon要求您發佈可用數量。 針對設定為不管理庫存但您想要在Amazon上列出的[!DNL Commerce]產品，此清單會以此處輸入值的可用數量發佈。 |

**快速存取** - [!UICONTROL Listing Settings]區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)

## 範例：最大列出數量

銷售料號時，Amazon清單會重新列出此數量。

例如，如果您將&#x200B;*[!UICONTROL Maximum Listed Quantity]*&#x200B;設為`12`，Amazon清單會顯示數量12，即使產品的[!DNL Commerce]數量為80也是如此：

![最大列出數量範例1](assets/amazon-max-listed-quantity.png){width="300"}

如果您將&#x200B;*[!UICONTROL Maximum Listed Quantity]*&#x200B;設為`1`，則所有合格產品都會列出，數量為`1`。 售出某個專案時，系統會尋找您的[!DNL Commerce]產品，如果有其他庫存，則會在Amazon上以`1`的數量重新搜尋該專案。

此選項對於通常訂購數量為1的產品可能很有價值。 這也增加了購物者在檢視Amazon清單時的急迫性。

![最大列出數量範例2](assets/amazon-max-listed-quantity-1.png){width="300"}
