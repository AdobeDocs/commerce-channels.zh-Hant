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

_[!UICONTROL Fulfilled By]_設定是您商店清單設定的一部分。 清單設定可從 [儲存儀表板](./amazon-store-dashboard.md).

這些設定定義履行（或發運）訂單的交易方。 如果您的所有訂單都使用一種方法履行，請在商家（您）或Amazon之間選擇。 如果您打算從您的地點完成訂單並使用Amazon，建議您使用第三個選項並設定 [!DNL Commerce] 產品屬性。

- **[!UICONTROL Fulfilled by Merchant]**  — 選擇您（商人）是否履行所有訂單。 下訂單時，系統會從 [!DNL Commerce] 目錄。

- **[!UICONTROL Fulfilled by Amazon]**  — 選擇Amazon是否滿足所有訂單。 使用此選項，產品詳細目錄不會從 [!DNL Commerce] 目錄。 Amazon已履行訂單的庫存庫存會儲存，並從其倉庫中扣除。 在指派此選項之前，您必須在 [!DNL Amazon Seller Central] 您的產品符合資格的帳戶 _由Amazon履行_ (FBA)完成。 FBA清單直接透過 [!DNL Amazon Seller Central] 帳戶。 透過此完成方法，Amazon銷售管道不會在 [!DNL Commerce] 和Amazon。 因此，並非所有數量設定中描述的行銷工具都可在Amazon銷售管道使用。

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]**  — 如果您的產品可能已由您和Amazon履行，您可以建立 [!DNL Commerce] 產品屬性，其值為「由商家履行」和「由Amazon履行」。 根據產品設定此值表示誰履行了訂單。

完成方法是區域屬性，並以 **[!UICONTROL Amazon Marketplace Country]** 設定 [商店整合](./store-integration.md). 進行變更時，此變更會影響所有共用該變更的Amazon清單 [!DNL Amazon Seller SKU] 在Amazon商店中銷售的相同地區(定義於 _[!UICONTROL Amazon Marketplace Country]_期間 [商店整合](./store-integration.md))。 對共用的變更 [!DNL Amazon Seller SKU] 在美國，不會影響您為不同地區設定的Amazon商店（如商店整合期間所定義）。

>[!NOTE]
>
>當訂單由Amazon(FBA)履行且已匯入訂單時，您可以在訂單詳細資料中看到某些欄位的虛擬資料。 請參閱 [Amazon訂單詳細資料](./amazon-order-details.md).

## 設定 [!UICONTROL Fulfilled By] 設定 {#configure-fulfilled-by-settings}

1. 按一下 **[!UICONTROL Listing Settings]** 在商店控制面板上。

1. 展開 _[!UICONTROL Fulfilled By]_區段。

1. 針對 **[!UICONTROL Product Fulfilled By]**，選擇完成（發運）順序：

   - `Fulfilled by Merchant`  — 商人履行命令。

   - `Fulfilled by Amazon` -Amazon倉庫符合訂單。

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] 屬性會指出誰符合每項產品的訂單。

      如果已選取，請選擇 [!DNL Commerce] 屬性 **[!UICONTROL Fulfilled by Attribute]**.

1. 完成後，按一下 **[!UICONTROL Save listing settings]**.

![完成者設定](assets/amazon-fulfilled-by.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | 選項：<ul><li>**[!UICONTROL Fulfilled by Merchant]** -(FBM)選擇是否完成訂單。 下訂單時，系統會從 [!DNL Commerce] 目錄。 建立新產品時，將分配「商戶已履行」的履行方法。</li><li>**[!UICONTROL Fulfilled by Amazon]** -(FBA)選擇Amazon是否滿足訂單。 使用此履行方法，產品庫存不會從 [!DNL Commerce] 目錄。 建立產品時，會使用 _[!UICONTROL Fulfilled by Amazon (FBA)]_作為履行類型。 確保您的產品符合FBA完成的資格， [!DNL Amazon Seller Central] 帳戶。 FBA庫存也直接透過 [!DNL Amazon Seller Central] 帳戶。 透過此履行方法，數量更新不會推送至您的 [!DNL Commerce] 目錄，因此您無法使用 [庫存/數量設定](./stock-quantity.md).</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]**  — 選擇是否有現有 [!DNL Commerce] 屬性，決定是由商家履行還是由Amazon履行。 選擇後， **[!UICONTROL Fulfilled by Attribute]** 啟用。</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 選擇 [!DNL Commerce] 用於確定履行方法的屬性。<br><br>例如，如果屬性為 _履行者_ 並選擇屬性值作為 _[!UICONTROL Fulfilled By Merchant]_或_[!UICONTROL Fulfilled By Amazon (FBA)]_，系統會將該值用作新產品的履行類型。 身為商家，您應確保您的產品符合在您的 [!DNL Amazon Seller Central] 帳戶。 FBA庫存也直接透過您的Amazon銷售商帳戶管理。<br><br>選項取決於您為Amazon產品設定的屬性。 |

**快速存取** - [!UICONTROL Listing Settings] 區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
