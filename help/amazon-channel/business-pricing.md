---
title: "[!DNL (B2B) Business Price] for Amazon清單"
description: 您可以在Amazon商業(B2B)網站上列出您的 [!DNL Commerce] 商店產品，方法是啟用Amazon [!DNL Seller Central] 帳戶中的商業。
role: Admin
level: Intermediate
feature: Sales Channels, Configuration, B2B, Tools and External Services, Merchandising, Integration
exl-id: 12a6cb2d-7a22-4b6d-9e94-ce91d564f42f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Amazon清單的[!DNL (B2B) Business Price]

(B2B)商業價格設定是商店清單設定的一部分。 清單設定可從[Amazon市集儀表板](./amazon-store-dashboard.md)存取。

[!DNL Amazon Business]是Amazon註冊企業帳戶專屬的市集，僅適用於美國、法國、德國和英國。 如果Marketplace允許B2B企業定價，則可在您的清單設定中進行編輯。

[!DNL B2B Business Pricing]可讓擁有商業帳戶的商戶以Amazon購物體驗的預期效能互相購買。 使用B2B業務定價，企業可以根據購買數量提供階層式定價。

若要讓您的產品列在[!DNL Amazon Business (B2B)]網站上，您必須先在[!DNL Amazon Seller Central]帳戶中啟用業務。 如需B2B功能的詳細資訊，請參閱[Amazon： B2B Central](https://sellercentral.amazon.com/gp/help/G202161480/){target="_blank"} （需要賣家中心登入）。

## 設定[!DNL (B2B) Business Price]設定

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Settings]**。

1. 展開&#x200B;_[!UICONTROL (B2B) Business Price]_區段。

1. 針對&#x200B;**[!UICONTROL Enable Business Pricing]**，選擇一個選項。

   - `Disabled` - （預設）當您不想啟用企業對企業的銷售時，請選擇此選項。 選擇後，此區段中的所有其他欄位都會停用。

   - `Enabled` — 選擇何時啟用企業對企業的銷售。 啟用時，業務價格會在套用所有訂價規則後設為等於定價。 業務價格會遵循網站訂價範圍（若已啟用）。 業務價格不得低於$1。

1. 針對&#x200B;**[!UICONTROL Enable Tiered Pricing]**，選擇一個選項。

   - `Disabled` - （預設）當您想要所有訂單數量使用相同的清單價格時，請選擇此選項。 選擇後，此區段中的所有&#x200B;_[!UICONTROL Pricing Level]_欄位都會停用。

   - `Enabled` — 選擇何時要根據訂單數量啟用訂價調整。 選擇後，會啟用&#x200B;_[!UICONTROL Pricing Level]_欄位。

1. 完成&#x200B;**[!UICONTROL Pricing Level]**&#x200B;設定。

   您可以定義最多5個數量/折扣設定，以設定業務清單的層級訂價。 在每個資料列中，輸入要套用的數量臨界值及折扣百分比。 例如，如果您在第一列的第一個欄位中輸入`5`，並在第二個欄位中輸入`5`，則當其他企業購買數量為5或以上時，價格會套用5%的折扣。

1. 完成時，按一下&#x200B;**[!UICONTROL Save listing settings]**。

![Amazon商業定價(B2B)](assets/amazon-business-pricing.png){width="500" zoomable="yes"}

| 欄位 | 說明 |
|----------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Enable Business Pricing] | 選項： <ul><li>**[!UICONTROL Disabled]** - （預設）當您不想啟用Business對Business銷售時，請選擇此選項。 選擇後，此區段中的所有其他欄位都會停用。</li><li>**[!UICONTROL Enabled]** — 選擇何時啟用業務對業務銷售。 選取時，業務價格會在套用所有訂價規則後設為等於定價。 業務價格會遵循網站訂價範圍（若已啟用）。 業務價格不得低於$1。</li></ul> |
| [!UICONTROL Enable Tiered Pricing] | （必要）選項： <ul><li>**[!UICONTROL Disabled]** - （預設）當您想要所有訂單數量使用相同的清單價格時，請選擇此選項。 選擇後，此區段中的所有&#x200B;_[!UICONTROL Pricing Level]_欄位都會停用。</li><li>**[!UICONTROL Enabled]** — 選擇何時啟用根據訂單數量調整的訂價。 選擇後，會啟用&#x200B;_[!UICONTROL Pricing Level]_欄位。</li></ul> |
| [!UICONTROL Pricing Level One-Five (qty/discount)] | 啟用「階層式訂價」時，您可以定義最多5個數量/折扣設定，以設定業務清單的階層式訂價。 在每個資料列中，輸入要套用的數量臨界值及折扣百分比。 例如，如果您在第一列的第一個欄位中輸入`5`，並在第二個欄位中輸入`5`，則當其他企業購買數量為5或以上時，價格會套用5%的折扣。 |

**快速存取** - [!UICONTROL Listing Settings]區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
