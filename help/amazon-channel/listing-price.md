---
title: 上市價格
description: 使用「清單價格」設定可確定您的Amazon清單的價格來源和基本（預設）價格值。
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 0%

---

# 上市價格

[!UICONTROL Listing Price] 設定是儲存清單設定的一部分。 從 [儲存儀表板](./amazon-store-dashboard.md)。

這些設定定義了 [!DNL Commerce] 定價屬性，用作您的價格來源，即您的Amazon清單的基本（預設）價格值。 這些設定由 [定價規則](./pricing-rule-general-settings.md) 自動調整您的Amazon清單價格，以 _[!UICONTROL Magento Price Source]_。

您可以配置 [定價範圍](./price-scope.md) 或網站。 如果定價範圍設定為 `Global`，您所有的商店/網站都有一個單一的價格來源。 如果定價範圍設定為 `Website`，價格來源使用網站價格（如果可用）的回退邏輯，然後使用預設（全局）價格。

如果將上市規則設定為應用於多個網站，則使用網站價格的順序由在 [清單規則](./listing-rules.md)。 這些規則允許您在目錄中定義產品定價。 要查看您是否在使用網站價格範圍，請參閱 [目錄價格範圍](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target="_blank"}。

中列出的選項 _[!UICONTROL Magento Price Source]_。_[!UICONTROL Minimum Advertised Price (Map)]_, _[!UICONTROL Strike Through Price (MSRP)]_包括您配置的定價屬性。 定價屬性為 [!DNL Commerce] 將「商店所有者的目錄輸入類型」值設定為的產品屬性 `Price`。 請參閱 [屬性輸入類型](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target="_blank"}。

## 配置清單價格設定 {#configure-listing-price-settings}

1. 按一下 **[!UICONTROL Listing Settings]** 在商店儀表板上。

1. 展開 _[!UICONTROL Listing Price]_的子菜單。

1. 對於 **[!UICONTROL Magento Price Source]** （必需），選擇選項。

   預設值為 `Price`。 此設定確定用於您的Amazon清單的價格來源。 如果建立 [定價規則](./pricing-products.md)，規則將應用於為此處選定的屬性定義的值。 您可以選擇任何已配置的定價屬性。 但是，如果未為產品填寫選定屬性，則產品的價格來源將預設回至 `Price` 定已公佈Amazon上市價格時釐定。

1. **[!UICONTROL Minimum Advertised Price (MAP)**]，也請參見Wiki頁。

   預設為無選擇。 此設定為產品啟用最低廣告價格(MAP)。 當您定義定價屬性且產品的上市價格低於您確定的最低價格（基於您的定價來源和規則）時，此值將成為上市的MAP。 此設定允許您實現 [定價規則](./pricing-products.md)，同時仍控制產品的最低價格。 要防止清單價格過低，請選擇要用作MAP的定價屬性。 但是，如果未為產品定義所選定價欄位，則不使用MAP。

1. 對於 **[!UICONTROL Strike Through Price (MSRP)]**，也請參見Wiki頁。

   預設為無選擇。 此設定確定哪個定價屬性用作產品的製造商建議零售價(MSRP)。 如果您的上市價格低於定義的MSRP，則顯示您的Amazon清單時會顯示MSRP價格的敲擊和較低的上市價格，以及計算的「您保存」金額和百分比。 但是，如果未為產品定義所選定價欄位，則不計算MSRP。

   >[!NOTE]
   >
   >此設定僅適用於已獲得 [Buy Box](./buy-box-competitor-pricing.md) 位置。 該Buy Box由Amazon授予銷售商，該銷售商的產品通常以最優惠的價格列出，同時還有其它因素，如FBA/Prime發貨量、供貨情況和銷售商的業績。

1. 對於 **應用增值稅**，選擇選項：

   - `Disabled`  — （預設）選擇您不想將增值稅應用於清單價格的時間。

   - `Enabled`  — 選擇要將增值稅應用於清單價格的時間。 增值稅通常用作歐洲國家的銷售稅，並添加到您在Amazon的最終標價中。 增值稅不適用於智慧定價規則內使用的清單的最終價格，除非 [底價](./floor-price.md) 命中。
   >[!NOTE]
   >
   >歐盟(EU)的企業需要向企業買家發送發票，以便客戶可以繳稅。 您可以自行生成這些發票並計算稅金，也可以使用稅務計算服務，如Amazon增值稅計算服務。 Amazon建議註冊 [Amazon增值稅計稅服務](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target="_blank"}。 如果您選擇了其他方法，則要對增值稅合規性負責。>
   >
   >Amazon可能需要10至14天時間驗證並激活您的增值稅計算服務帳戶。

1. 對於 **[!UICONTROL VAT Percentage]**，輸入增值稅稅率的值。

   預設值為 `0.00`。 此值用於計算要添加到上市價格的增值稅金額。 如果 `10.2` 輸入時，您的上市價格將應用10.20%的增值稅。 將「應用增值稅(VAT)」欄位設定為時，此欄位將禁用 `Disabled`。

1. **（僅限英國商店）** 對於 **[!UICONTROL Amazon Product Tax Code (PTC)]**，選擇選項：

   - `Do Not Manage PTC`  — （預設）選擇您是使用第三方計稅服務，還是已在您的 [!DNL Amazon Seller Central] 帳戶。 選擇後，Amazon銷售渠道不會向您的 [!DNL Amazon Seller Central] 帳戶。

   - `Set Default PTC`  — 選擇是否具有要用於所有產品的通用產品稅碼(PTC)。 選擇後，必須完成 _[!UICONTROL Default PTC]_。

      - 對於 **[!UICONTROL Default PTC]**，輸入要用於所有合格的Amazon清單的預設PTC。 如果在中設定了預設PTC [!DNL Amazon Seller Central] 帳戶，將此欄位留空。 對此欄位所做的更改不會影響現有的Amazon清單。 要更改現有清單的「預設PTC」(Default PTC)，該清單必須 [截止](./end-listings-manually.md) 並建立新清單。
   >[!NOTE]
   >
   >如果使用Amazon增值稅計算服務，則必須知道產品的稅種。 PTC是Amazon在歐盟B2B採購的稅種ID代碼。 請參閱 [Amazon的產品稅碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}。

1. 對於 **[!UICONTROL Currency Conversion]**，也請參見Wiki頁。

   預設值為 `Disabled`。 這些選項取決於您 [!DNL Commerce] [貨幣](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target="_blank"} 的子菜單。 如果沒有可用選項，請設定貨幣設定。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**。

![上市價格](assets/amazon-listing-price.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Magento Price Source] | 確定在建立Amazon清單時使用的價格來源。 預設值為 `Price`。 如果您選擇其他屬性，如 `Amazon Price` 或 `Special Price`，該屬性的定義值用於您的Amazon清單。 但是，如果未定義選定屬性， `Price` 的子菜單。 |
| [!UICONTROL Minimum Advertised Price (MAP)] | 的 [!DNL Commerce] 屬性。 如果MAP價格低於MAP價格，選擇MAP選項會自動將您的Amazon清單設定為MAP價格。 |
| [!UICONTROL Strike Through Price (MSRP)] | 的 [!DNL Commerce] 表示MSRP定價的屬性。 如果您的Amazon上市價格低於MSRP，則顯示MSRP價格和上市價格的全面執行。 此設定還用於計算「您保存」金額和百分比，但此功能僅適用於已獲得 [Buy Box](./buy-box-competitor-pricing.md) 位置。 |
| [!UICONTROL Apply Value Added Tax (VAT)] | 歐盟的賣方使用增值稅。<br><br>選擇 `Disabled` 如果您不想將增值稅添加到列價中。<br><br>選擇 `Enabled` 然後輸入增值稅百分比，以將增值稅應用於您的清單價格。 |
| [!UICONTROL VAT Percentage] | 定義用於計算要添加到您的Amazon清單的清單價格的增值稅金額的百分比。 <br><br>如果輸入 `5`，則於應用所有定價規則後，對最終上市價格應用5%的增值稅。 增值稅不適用於智慧定價規則內使用的清單的最終價格，除非 [地板](./floor-price.md) 或 [天花板](./optional-ceiling-price.md) 命中。 |
| [!UICONTROL Amazon Product Tax Code (PTC)] | （僅用於英國商店）確定Amazon銷售渠道是否將產品稅碼資訊發送給您 [!DNL Amazon Seller Central] 帳戶。 <br><br>選擇 **不管理PTC** 如果您使用第三方稅務計算服務，或已在您的 [!DNL Amazon Seller Central] 帳戶。 如果設定為此選項，Amazon銷售渠道將不向您發送產品稅碼資訊 [!DNL Amazon Seller Central] 帳戶。<br><br>選擇 **設定預設PTC** 如果您具有通用產品稅碼，則您希望用於所有產品。<br><br>請參閱 [Amazon的產品稅碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}。 |
| [!UICONTROL Default PTC] | 僅在 **Amazon產品稅碼(PTC)** 設定為 `Set Default PTC`。 輸入要用於所有符合條件的Amazon清單的預設PTC。 如果在中設定了預設PTC [!DNL Amazon Seller Central] 帳戶，將此欄位留空。 <br><br>對此欄位所做的更改不會影響現有清單。 清單必須為 [截止](./end-listings-manually.md) 以及為更改生效而建立的新清單。 |
| [!UICONTROL Currency Conversion] | 允許 [!DNL Commerce] storefront預設貨幣，以準確兌換為預設的Amazon貨幣，以適當的貨幣發佈清單價格。 貨幣兌換始終基於 [!DNL Commerce] 預設貨幣。<br><br>您仍可以查看預設 [!DNL Commerce] 以及Amazon貨幣。 如果預設 [!DNL Commerce] 貨幣與預設的Amazon貨幣匹配，請禁用「貨幣兌換」。<br><br>例如，如果 [!DNL Commerce] 預設貨幣為CAD（加元），而Amazon預設貨幣為USD，您必須啟用「幣種折換」並選擇「折換率CAD至USD」。 所呈列之選項乃根據 [!DNL Commerce] 貨幣兌換。 如果你看不到你想要的選項， [在中設定貨幣 [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target="_blank"}。 |

**快速訪問** - [!UICONTROL Listing Settings] 節

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
