---
title: 上市價
description: 使用「上市價格」設定來判斷您的Amazon清單的價格來源和基本（預設）價格值。
redirect_from: sales-channels/asc/ob-listing-price.html
exl-id: d97d81fa-c298-423f-9072-050ee72e707e
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 上市價

[!UICONTROL Listing Price] 設定是您商店清單設定的一部分。清單設定可從[儲存控制面板](./amazon-store-dashboard.md)存取。

這些設定會定義要用作價格來源的[!DNL Commerce]定價屬性，這是您Amazon清單的基礎（預設）價格值。 您的[定價規則](./pricing-rule-general-settings.md)會使用這些設定，以根據為&#x200B;_[!UICONTROL Magento Price Source]_設定的值自動調整您的Amazon清單價格。

您可以將[定價範圍](./price-scope.md)配置為全局或網站。 如果您的定價範圍設定為`Global`，則所有商店/網站都有單一價格來源。 如果您的定價範圍設為`Website`，則價格來源會使用網站價格的後援邏輯（如果有），後跟預設（全域）價格。

如果將清單規則設定為應用於多個網站，則使用網站價格的順序由[清單規則](./listing-rules.md)中定義的網站優先順序設定確定。 這些規則可讓您定義目錄中的產品定價。 若要查看您是否使用網站價格範圍，請參閱[目錄價格範圍](https://docs.magento.com/user-guide/catalog/catalog-price-scope.html){target=&quot;_blank&quot;}。

_[!UICONTROL Magento Price Source]_、_[!UICONTROL Minimum Advertised Price (Map)]_&#x200B;和&#x200B;_[!UICONTROL Strike Through Price (MSRP)]_中列出的選項包括您配置的定價屬性。 定價屬性是[!DNL Commerce]產品屬性，「商店所有者」值的「目錄輸入類型」設定為`Price`。 請參閱[屬性輸入類型](https://docs.magento.com/user-guide/stores/attributes-input-types.html){target=&quot;_blank&quot;}。

## 配置清單價格設定 {#configure-listing-price-settings}

1. 按一下儲存控制面板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL Listing Price]_區段。

1. 對於&#x200B;**[!UICONTROL Magento Price Source]**（必要），選擇一個選項。

   預設值為`Price`。 此設定會決定用於Amazon清單的價格來源。 如果建立[定價規則](./pricing-products.md)，則規則將應用於為此處選擇的屬性定義的值。 您可以選擇任何配置的定價屬性。 不過，如果未填入產品的選定屬性，則應用定價規則以確定已發佈的Amazon上市價格時，產品的價格來源預設回`Price`。

1. 對於**[!UICONTROL Minimum Advertised Price (MAP)**]，選擇一個選項。

   預設值為無選取項目。 此設定可為產品啟用最低廣告價格(MAP)。 當您定義定價屬性，而產品的上市價格低於您確定的最低價格時（根據您的定價來源和規則），此值將成為上市的MAP。 此設定可讓您實作[定價規則](./pricing-products.md)，同時仍控制產品的最低價格。 要防止上市價格過低，請選擇要用作MAP的定價屬性。 但是，如果未為產品定義所選定價欄位，則不使用MAP。

1. 對於&#x200B;**[!UICONTROL Strike Through Price (MSRP)]**，選擇一個選項。

   預設值為無選取項目。 此設定會決定使用哪個定價屬性作為產品的製造商建議零售價(MSRP)。 如果您的上市價格低於定義的MSRP，則您的Amazon清單會以較低的上市價格以及計算的「您節省」金額和百分比顯示MSRP價格的實際執行。 不過，如果未為產品定義選取的定價欄位，則不會計算MSRP。

   >[!NOTE]
   >
   >此設定僅適用於獲得[Buy Box](./buy-box-competitor-pricing.md)位置的清單。 該Buy Box由Amazon授予銷售商，該銷售商將產品以通常最優惠的價格上市，並搭配其他因素，如FBA/Prime的出貨量、供貨情況和銷售商的業績。

1. 對於&#x200B;**應用增值稅(VAT)**，選擇一個選項：

   - `Disabled`  — （預設）選擇您不想將增值稅套用至上市價格的時間。

   - `Enabled`  — 選擇何時將增值稅應用到上市價格。VAT通常在歐洲國家/地區用作銷售稅，並加到您在Amazon內的最終上市價格中。 增值稅不適用於智慧定價規則內使用之清單的最終價格，除非[底價](./floor-price.md)已點擊。
   >[!NOTE]
   >
   >歐盟(EU)的企業必須將發票發送給企業買家，以便客戶可以匯稅。 您可以自行生成這些發票並計算稅金，或使用稅金計算服務，如Amazon的增值稅計算服務。 Amazon建議註冊[Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources?ref_=asuk_soa_rd&amp;){target=&quot;_blank&quot;}。 如果您選擇其他方法，則需對增值稅法規遵從負責。>
   >
   >Amazon可能需要10到14天的時間來驗證和啟用您的增值稅計算服務帳戶。

1. 對於&#x200B;**[!UICONTROL VAT Percentage]**，輸入增值稅稅率的值。

   預設值為`0.00`。 此值用於計算要添加到掛起價格中的增值稅金額。 如果輸入了`10.2`，則對您的清單價格應用10.20%的增值稅。 當「應用增值稅(VAT)」欄位設定為`Disabled`時，此欄位將被禁用。

1. **（僅限英國商店）** 若 **[!UICONTROL Amazon Product Tax Code (PTC)]**&#x200B;要選擇一個選項：

   - `Do Not Manage PTC`  — （預設）選擇您是使用第三方計稅服務，還是已在您的帳戶中設定了所有計 [!DNL Amazon Seller Central] 稅。選擇後，Amazon銷售管道不會將任何產品稅碼資訊傳送至您的[!DNL Amazon Seller Central]帳戶。

   - `Set Default PTC`  — 選擇是否具有要用於所有產品的通用產品稅碼(PTC)。選擇後，必須完成&#x200B;_[!UICONTROL Default PTC]_。

      - 對於&#x200B;**[!UICONTROL Default PTC]**，輸入要用於所有符合條件的Amazon清單的預設PTC。 如果在[!DNL Amazon Seller Central]帳戶中設定了預設PTC，請將此欄位留空。 對此欄位所做的變更不會影響現有的Amazon清單。 要更改現有清單的「預設PTC」，清單必須是[ended](./end-listings-manually.md)並建立新清單。
   >[!NOTE]
   >
   >如果您使用Amazon的增值稅計算服務，則必須知道產品的稅種。 PTC是Amazon在歐盟的B2B採購稅類別ID代碼。 請參閱[Amazon的產品稅碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}。

1. 對於&#x200B;**[!UICONTROL Currency Conversion]**，選擇一個選項。

   預設值為`Disabled`。 這些選項取決於您的[!DNL Commerce] [currency](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;}設定。 如果沒有可用選項，請設定貨幣設定。

1. 完成後，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![上市價](assets/amazon-listing-price.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Magento Price Source] | 決定建立Amazon清單時使用的價格來源。 預設值為`Price`。 如果您選擇其他屬性，例如`Amazon Price`或`Special Price`，則該屬性的定義值會用於Amazon清單。 但是，如果未定義所選屬性，則使用`Price`。 |
| [!UICONTROL Minimum Advertised Price (MAP)] | MAP定價的[!DNL Commerce]屬性。 如果上市價格低於MAP價格，選擇MAP選項會自動將您的Amazon上市設定為MAP價格。 |
| [!UICONTROL Strike Through Price (MSRP)] | 代表MSRP定價的[!DNL Commerce]屬性。 如果您的Amazon上市價格低於MSRP，則會顯示MSRP價格和上市價格的執行。 此設定也用於計算「您保存」金額和百分比，但此功能僅適用於獲得[Buy Box](./buy-box-competitor-pricing.md)位置的清單。 |
| [!UICONTROL Apply Value Added Tax (VAT)] | VAT供歐盟的銷售者使用。<br><br>如 `Disabled` 果不想將增值稅添加到清單價格中，請選擇。<br><br>選 `Enabled` 擇，然後輸入增值稅百分比，以將增值稅應用於清單價格。 |
| [!UICONTROL VAT Percentage] | 定義要用於計算要新增至Amazon清單上市價格的增值稅金額的百分比。 <br><br>如果輸 `5`入，則在應用所有定價規則後，系統將對最終上市價格應用5%的增值稅。增值稅不適用於智慧定價規則內使用的清單的最終價格，除非點擊[floor](./floor-price.md)或[ceiling](./optional-ceiling-price.md)。 |
| [!UICONTROL Amazon Product Tax Code (PTC)] | （僅針對英國商店顯示）判斷Amazon銷售管道是否將產品稅碼資訊傳送至您的[!DNL Amazon Seller Central]帳戶。 <br><br>如果 **您使用第** 三方計稅服務，或已在您的帳戶中設定了所有計稅，請選擇「不管理PTC [!DNL Amazon Seller Central] 」。設為此選項時，Amazon銷售管道不會將產品稅碼資訊傳送至您的[!DNL Amazon Seller Central]帳戶。<br><br>如果 **您有要** 用於所有產品的通用產品稅碼，請選擇「設定預設PTC」。<br><br>請參 [閱Amazon的產品稅碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target=&quot;_blank&quot;}。 |
| [!UICONTROL Default PTC] | 僅當&#x200B;**Amazon產品稅碼(PTC)**&#x200B;設定為`Set Default PTC`時才顯示。 輸入要用於所有合格Amazon清單的預設PTC。 如果在[!DNL Amazon Seller Central]帳戶中設定了預設PTC，請將此欄位留空。 <br><br>對此欄位所做的更改不會影響現有清單。清單必須是[ended](./end-listings-manually.md)，並建立新清單，變更才會生效。 |
| [!UICONTROL Currency Conversion] | 允許您的[!DNL Commerce]店面預設貨幣準確轉換為預設的Amazon貨幣，以發佈使用適當貨幣的清單價格。 貨幣轉換一律以您的[!DNL Commerce]預設貨幣為基礎。<br><br>當其他貨幣可用時，您 [!DNL Commerce] 仍可以檢視預設貨幣和Amazon貨幣。如果您的預設[!DNL Commerce]貨幣符合您的預設Amazon貨幣，請停用「貨幣轉換」。<br><br>例如，如果預設貨 [!DNL Commerce] 幣為CAD（加元），而Amazon預設貨幣為USD，則必須啟用「貨幣轉換」，然後選擇「折換率CAD為USD」。所呈現的選項是以內建的[!DNL Commerce]貨幣轉換為基礎。 如果您沒有看到要尋找的選項，請[在 [!DNL Commerce]](https://docs.magento.com/user-guide/stores/currency-configuration.html){target=&quot;_blank&quot;}中設定貨幣。 |

**快速存取**  — 區 [!UICONTROL Listing Settings] 段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
