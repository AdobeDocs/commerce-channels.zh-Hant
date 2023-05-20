---
title: 履行者
description: 使用「履行者」設定確定如何履行Amazon清單中的訂單（已發運）。
redirect_from: /sales-channels/asc/ob-fulfilled-by.html
exl-id: 240c2198-e23d-40e7-be39-b9a4f78565d2
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# 履行者

_[!UICONTROL Fulfilled By]_設定是儲存清單設定的一部分。 從 [儲存儀表板](./amazon-store-dashboard.md)。

這些設定定義履行（或發運）訂單的當事方。 如果您的所有訂單都使用一種方法履行，請在商家（您）或Amazon之間進行選擇。 如果您計畫從您的地點完成訂單並使用Amazon，則最好使用第三個選項並配置 [!DNL Commerce] 產品屬性。

- **[!UICONTROL Fulfilled by Merchant]**  — 選擇您（商戶）是否履行所有訂單。 下單時，庫存將從 [!DNL Commerce] 目錄。

- **[!UICONTROL Fulfilled by Amazon]**  — 選擇Amazon是否履行所有訂單。 使用此選項，產品庫存不會從 [!DNL Commerce] 下訂單時編錄。 Amazon已履行訂單的庫存庫存被儲存並從其倉庫扣除。 在分配此選項之前，必須在 [!DNL Amazon Seller Central] 您的產品符合資格的帳戶 _由Amazon履行_ 完成。 FBA庫存直接通過 [!DNL Amazon Seller Central] 帳戶。 使用此完成方法，Amazon銷售渠道不在兩個渠道之間共用數量更新 [!DNL Commerce] 和Amazon。 因此，並非所有數量設定中描述的市場營銷工具都可在Amazon銷售渠道中獲得。

- **[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]**  — 如果您的產品可能由您和Amazon完成，您可能希望建立 [!DNL Commerce] 具有「按商戶履行」和「按Amazon履行」值的產品屬性。 按產品設定此值表示誰履行了訂單。

完成方法是一種區域屬性，並基於 **[!UICONTROL Amazon Marketplace Country]** 設定在 [儲存整合](./store-integration.md)。 當進行更改時，該更改將影響共用該更改的所有Amazon上市 [!DNL Amazon Seller SKU] 在你Amazon的店裡銷售的 _[!UICONTROL Amazon Marketplace Country]_在 [儲存整合](./store-integration.md))。 對共用的更改 [!DNL Amazon Seller SKU] 在美國，不會影響您為不同區域設定的Amazon商店（如在商店整合期間定義的）。

>[!NOTE]
>
>當訂單由Amazon(FBA)完成且訂單已導入時，您可以在訂單詳細資訊中看到某些欄位的虛擬資料。 請參閱 [Amazon訂單詳細資訊](./amazon-order-details.md)。

## 配置 [!UICONTROL Fulfilled By] 設定 {#configure-fulfilled-by-settings}

1. 按一下 **[!UICONTROL Listing Settings]** 在商店儀表板上。

1. 展開 _[!UICONTROL Fulfilled By]_的子菜單。

1. 對於 **[!UICONTROL Product Fulfilled By]**，選擇完成（發運）訂單的人：

   - `Fulfilled by Merchant`  — 商人履行訂單。

   - `Fulfilled by Amazon` -Amazon倉庫履行訂單。

   - `Assign Fulfilled By Using Magento Product Attribute` - A [!DNL Commerce] 屬性指明誰按產品履行訂單。

      如果選擇，請選擇 [!DNL Commerce] 要映射的屬性 **[!UICONTROL Fulfilled by Attribute]**。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**。

![按設定完成](assets/amazon-fulfilled-by.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Product Fulfilled By] | 選項：<ul><li>**[!UICONTROL Fulfilled by Merchant]** -(FBM)選擇是否完成訂單。 下單時，庫存將從 [!DNL Commerce] 目錄。 在建立新產品時，將分配「商家履行」的履行方法。</li><li>**[!UICONTROL Fulfilled by Amazon]** -(FBA)選擇Amazon是否履行訂單。 使用此完成方法，產品庫存不會從您的 [!DNL Commerce] 下訂單時編錄。 建立產品時，將使用 _[!UICONTROL Fulfilled by Amazon (FBA)]_作為履行類型。 確保您的產品符合FBA履行條件 [!DNL Amazon Seller Central] 帳戶。 FBA庫存也通過您的 [!DNL Amazon Seller Central] 帳戶。 使用此完成方法，數量更新不會相對於您的 [!DNL Commerce] 目錄，因此不能使用中介紹的一些營銷工具 [庫存/數量設定](./stock-quantity.md)。</li><li>**[!UICONTROL Assign Fulfilled By Using Magento Product Attribute]**  — 選擇是否具有現有 [!DNL Commerce] 屬性，確定是由商戶履行還是由Amazon履行。 選擇後， **[!UICONTROL Fulfilled by Attribute]** 啟用。</li></ul> |
| [!UICONTROL Fulfilled By Attribute] | 選擇 [!DNL Commerce] 用於確定履行方法的屬性。<br><br>例如，如果屬性 _履行者_ 然後選擇屬性值作為 _[!UICONTROL Fulfilled By Merchant]_或_[!UICONTROL Fulfilled By Amazon (FBA)]_，系統將該值用作新產品的履行類型。 作為商家，您應確保您的產品符合FBA履行條件 [!DNL Amazon Seller Central] 帳戶。 FBA庫存也通過您的Amazon銷售商帳戶直接管理。<br><br>選項取決於您為Amazon產品設定的屬性。 |

**快速訪問** - [!UICONTROL Listing Settings] 節

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
