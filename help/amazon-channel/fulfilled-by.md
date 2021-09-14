---
title: 履行者
description: 使用「履行者」設定來判斷如何履行Amazon清單中的訂單（已發運）。
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# 履行者

_[!UICONTROL Fulfilled By]_設定是您商店清單設定的一部分。清單設定可從[儲存控制面板](./amazon-store-dashboard.md)存取。

這些設定定義履行（或發運）訂單的交易方。 如果您的所有訂單都使用一種方法履行，請在商家（您）或Amazon之間選擇。 如果您打算從您的地點完成訂單並使用Amazon，最好使用第三個選項並設定[!DNL Commerce]產品屬性。

- **[!UICONTROL Fulfilled by Merchant]**  — 選擇您（商人）是否履行所有訂單。下訂單時，庫存將從[!DNL Commerce]目錄中扣除。

- **[!UICONTROL Fulfilled by Amazon]**  — 選擇Amazon是否滿足所有訂單。使用此選項，下單時不會從[!DNL Commerce]目錄中扣除產品庫存。 Amazon已履行訂單的庫存庫存會儲存，並從其倉庫中扣除。 在分配此選項之前，您必須在[!DNL Amazon Seller Central]帳戶中驗證您的產品是否符合由Amazon _(FBA)履行的資格。_ FBA清單直接透過您的[!DNL Amazon Seller Central]帳戶管理。 透過此履行方法，Amazon銷售管道不會在[!DNL Commerce]與Amazon之間共用數量更新。 因此，並非所有數量設定中描述的行銷工具都可在Amazon銷售管道使用。

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]**  — 如果您的產品可能由您和Amazon履行，您可能想要建立產品屬性，其 [!DNL Commerce] 中包含「由商家履行」和「由Amazon履行」的值。根據產品設定此值表示誰履行了訂單。

實現方法是區域屬性，且以[儲存整合](./store-integration.md)期間定義的&#x200B;**[!UICONTROL Amazon Marketplace Country]**&#x200B;設定為基礎。 進行變更時，變更會影響在您的Amazon商店中共用該[!DNL Amazon Seller SKU]的所有Amazon清單，這些清單在相同地區銷售（如&#x200B;_[!UICONTROL Amazon Marketplace Country]_期間[商店整合](./store-integration.md)中所定義）。 在美國對共用[!DNL Amazon Seller SKU]所做的變更不會影響您為不同區域設定的Amazon商店（如商店整合期間所定義）。

>[!NOTE]
>
>當訂單由Amazon(FBA)履行且已匯入訂單時，您可以在訂單詳細資料中看到某些欄位的虛擬資料。 請參閱[Amazon訂單詳細資料](./amazon-order-details.md)。

## 配置[!UICONTROL Fulfilled By]設定 {#configure-fulfilled-by-settings}

1. 按一下儲存控制面板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Fulfilled By]_區段。

1. 對於&#x200B;**[!UICONTROL Product Fulfilled By]**，選擇完成（發運）訂單的人員：

   - `Fulfilled by Merchant`  — 商人履行命令。

   - `Fulfilled by Amazon` -Amazon倉庫符合訂單。

   - `Assign Fulfilled By Using Magento Product Attribute`  — 屬性 [!DNL Commerce] 指示誰滿足每項產品的訂單。

      如果選擇了，請選擇&#x200B;**[!UICONTROL Fulfilled by Attribute]**&#x200B;中要映射的[!DNL Commerce]屬性。

1. 完成後，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![完成者設定](assets/amazon-fulfilled-by.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | 選項：<ul><li>**[!UICONTROL Fulfilled by Merchant]** -(FBM)選擇是否完成訂單。下訂單時，庫存將從[!DNL Commerce]目錄中扣除。 建立新產品時，將分配「商戶已履行」的履行方法。</li><li>**[!UICONTROL Fulfilled by Amazon]** -(FBA)選擇Amazon是否滿足訂單。使用此完成方法，在下訂單時，產品庫存不會從[!DNL Commerce]目錄中扣除。 建立產品時，會以&#x200B;_[!UICONTROL Fulfilled by Amazon (FBA)]_建立該產品，作為履行類型。 確保您的產品符合[!DNL Amazon Seller Central]帳戶內的FBA履行資格。 FBA清單也直接透過您的[!DNL Amazon Seller Central]帳戶管理。 使用此履行方法時，數量更新不會相對於您的[!DNL Commerce]目錄推出，因此您無法使用[庫存/數量設定](./stock-quantity.md)中所述的某些行銷工具。</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]**  — 選擇您是否有現有屬 [!DNL Commerce] 性，以決定是由商戶履行還是由Amazon履行。選擇&#x200B;**[!UICONTROL Fulfilled by Attribute]**&#x200B;後啟用。</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 選擇用於確定履行方法的[!DNL Commerce]屬性。<br><br>例如，如果屬性為「 _履行_ 者」，而您選擇屬性值 _[!UICONTROL Fulfilled By Merchant]_為或_[!UICONTROL Fulfilled By Amazon (FBA)]_，則系統會將該值用作新產品的履行類型。身為商家，您應確保您的產品符合[!DNL Amazon Seller Central]帳戶內的FBA履行資格。 FBA庫存也直接透過您的Amazon銷售商帳戶管理。<br><br>選項取決於您為Amazon產品設定的屬性。 |

**快速存取**  — 區 [!UICONTROL Listing Settings] 段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
