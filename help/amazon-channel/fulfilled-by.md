---
title: Amazon清單的完成者設定
description: 使用「履行者」設定來決定如何履行（出貨）Amazon清單中的訂單。
feature: Sales Channels, Products
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Amazon清單的完成者設定

_[!UICONTROL Fulfilled By]_設定是商店清單設定的一部分。 清單設定可從[存放區儀表板](./amazon-store-dashboard.md)存取。

這些設定會定義履行（或出貨）訂單的合作對象。 如果您的所有訂單都是使用單一方式完成，請在特約商（您）或Amazon之間選擇。 如果您打算完成您所在位置的訂單並使用Amazon，最佳做法是使用第三個選項並設定[!DNL Commerce]產品屬性。

- **[!UICONTROL Fulfilled by Merchant]** — 選擇您（商人）是否履行所有訂單。 下訂單時，存貨會從您的[!DNL Commerce]目錄中扣除。

- **[!UICONTROL Fulfilled by Amazon]** — 選擇Amazon是否履行所有訂單。 使用此選項，下訂單時不會從您的[!DNL Commerce]目錄中扣除產品詳細目錄。 Amazon已履行訂單的存貨存量會儲存並從其倉庫中扣除。 指派此選項之前，您必須先在您的[!DNL Amazon Seller Central]帳戶中確認您的產品符合&#x200B;_由Amazon履行_ (FBA)的履行資格。 透過您的[!DNL Amazon Seller Central]帳戶直接管理FBA詳細目錄。 使用此履行方法，Amazon銷售管道不會在[!DNL Commerce]和Amazon之間共用數量更新。 因此，並非所有數量設定中所述的行銷工具都可以在Amazon銷售管道中使用。

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** — 如果您的產品可能由您和Amazon履行，您可以建立[!DNL Commerce]產品屬性，其值為「由商家履行」和「由Amazon履行」。 若為每個產品設定此值，表示誰將履行訂單。

履行方法是區域屬性，且以[存放區整合](./store-integration.md)期間定義的&#x200B;**[!UICONTROL Amazon Marketplace Country]**&#x200B;設定為基礎。 進行變更時，此變更會影響在您的Amazon商店中分享[!DNL Amazon Seller SKU]並在相同地區銷售之所有Amazon清單（在[商店整合](./store-integration.md)期間於&#x200B;_[!UICONTROL Amazon Marketplace Country]_中定義）。 在美國對共用[!DNL Amazon Seller SKU]的變更不會影響您為其他區域設定的Amazon存放區（如存放區整合期間所定義）。

>[!NOTE]
>
>當訂單由Amazon (FBA)履行且已匯入訂單時，您可能會在訂單詳細資料中看到某些欄位的虛擬資料。 請參閱[Amazon訂單詳細資料](./amazon-order-details.md)。

## 設定[!UICONTROL Fulfilled By]設定 {#configure-fulfilled-by-settings}

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Fulfilled By]_區段。

1. 針對&#x200B;**[!UICONTROL Product Fulfilled By]**，選擇履行（出貨）訂單的人員：

   - `Fulfilled by Merchant` — 商家履行訂單。

   - `Fulfilled by Amazon` - Amazon倉儲履行訂單。

   - `Assign Fulfilled By Using Magento Product Attribute` - [!DNL Commerce]屬性指出誰能完成每個產品的訂單。

     若已選擇，請選擇您要在&#x200B;**[!UICONTROL Fulfilled by Attribute]**&#x200B;中對應的[!DNL Commerce]屬性。

1. 完成時，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![由設定完成](assets/amazon-fulfilled-by.png){width="500" zoomable="yes"}

| 欄位 | 說明 |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product Fulfilled By] | 選項：<ul><li>**[!UICONTROL Fulfilled by Merchant]** - (FBM)選擇是否履行訂單。 下訂單時，存貨會從您的[!DNL Commerce]目錄中扣除。 建立新產品時，會指派「已履行的商家」的履行方法。</li><li>**[!UICONTROL Fulfilled by Amazon]** - (FBA)選擇Amazon是否履行訂單。 使用此履行方法，下訂單時不會從您的[!DNL Commerce]目錄中扣除產品詳細目錄。 建立產品時，會以&#x200B;_[!UICONTROL Fulfilled by Amazon (FBA)]_作為履行型別來建立產品。 確保您的產品符合[!DNL Amazon Seller Central]帳戶中的FBA履行資格。 FBA詳細目錄也透過您的[!DNL Amazon Seller Central]帳戶直接管理。 使用此履行方法，不會推出相對於您[!DNL Commerce]目錄的數量更新，因此您無法使用[庫存/數量設定](./stock-quantity.md)中說明的某些行銷工具。</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]** — 選擇您是否擁有現有的[!DNL Commerce]屬性，以判斷它是由商家履行或由Amazon履行。 選擇後，**[!UICONTROL Fulfilled by Attribute]**&#x200B;會啟用。</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 選擇用來決定履行方法的[!DNL Commerce]屬性。<br><br>例如，如果屬性是&#x200B;_履行者_，而您選擇屬性值為`Fulfilled By Merchant`或`Fulfilled By Amazon (FBA)`，則系統將該值作為新產品的履行型別。 身為商家，您應該確保您的產品符合[!DNL Amazon Seller Central]帳戶中的FBA履行資格。 FBA詳細目錄也可透過您的Amazon賣家帳戶直接管理。<br><br>選項取決於您為Amazon產品設定的屬性。 |

**快速存取** - [!UICONTROL Listing Settings]區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
