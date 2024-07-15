---
title: Amazon清單的預設商店設定
description: 修改預設Commerce設定，以自訂您商店的AmazonSales Channel。
role: Admin
feature: Sales Channels, Integration, Configuration
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Amazon清單的預設商店設定

您的商店連線並設定好第一個清單規則後，Amazon與[!DNL Commerce]之間的資料同步就會開始。 有多種型別的商店設定可讓您根據需求自訂商店。 在存放區[儀表板](./amazon-store-dashboard.md)上存取存放區設定。

商店設定包括：

- [**[!UICONTROL Listing settings]**](./listing-settings.md) — 控制您的產品目錄與[!DNL Amazon Marketplace]互動的方式。

- [**[!UICONTROL Order settings]**](./order-settings.md) — 控制Amazon訂單的管理方式。

- [**[!UICONTROL Listing rules]**](./listing-rules.md) — 定義哪些目錄產品符合在Amazon上列出的資格。

- [**[!UICONTROL Pricing rules]**](./pricing-products.md) — 定義如何變更合格清單的Amazon定價。

- **[!UICONTROL Store reports]** - [競爭價格分析](./competitive-price-analysis.md)和[清單改進](./listing-improvements.md)。

- **[!UICONTROL Logs]** - [清單變更](./listing-changes-log.md)和[通訊錯誤](./communication-errors-log.md)。

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md) — 檢閱[!DNL Commerce]管理員中的電子郵件和Amazon銷售管道商店名稱設定。

## 一些重要的預設設定

| 設定 | 預設 | 說明 | 位置 |
|----------------------------------------|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| [!UICONTROL Import Amazon Orders] | `Enabled` | 從Amazon收到新訂單時，建立對應的[!DNL Commerce]訂單，允許在[[!DNL Commerce] 訂單](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/orders/orders.html)工作流程中管理訂單。 當`Disabled`時，Amazon訂單匯入訂單資訊以供檢閱，但必須在您的[!DNL Amazon Seller Central]帳戶中管理訂單。 | [訂單設定](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | 來自Amazon訂單的客戶資料未匯入您的[!DNL Commerce]資料庫。 匯入的Amazon訂單會作為訪客結帳處理。 若要建置[!DNL Commerce]客戶資料庫，您應該將此設定變更為`Build New Customer Account`。 | [訂單設定](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce]個目錄產品(符合Amazon的資格要求)以自動發佈至Amazon並建立Amazon清單。 如果您想要手動檢閱並發佈您的產品，您應該將此設定變更為`Do Not Automatically List Eligible Products`。 等待手動發佈的產品會顯示在&#x200B;[_準備清單_](./ready-to-list.md)&#x200B;索引標籤上。 | [產品清單動作](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | 定義作為Amazon清單基礎的價格來源屬性。 如果您不想使用[!DNL Commerce] `Price`屬性作為您的訂價規則所依據的基準價格，您應該將此設定變更為其他屬性。 | [清單價格](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | 商家會履行所有訂單。 如果您使用Amazon的Fulfillment或使用多種履行方法，則應變更此設定。 | [履行者：](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | 如果您的所有產品條件相同，您可以選取其中一個Amazon條件選項來代表您的所有產品。 如果您的目錄包含不同條件的產品（例如「新增」、「已使用」及「已翻新」），您必須將此設定變更為「`Assign Condition Using Product Attribute`」，並將「[!DNL Commerce]」條件屬性對應至您的Amazon清單條件。 | [產品清單條件](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | 無 | 定義用來決定Amazon銷售管道會將哪些產品發佈至Amazon的規則。 這些規則提供許多選項，可建立從簡單到複雜的規則，以將產品納入或排除為清單。 | [清單規則](./listing-rules.md) |
| 訂價規則 | 無 | 定義您的Amazon清單價格屬性，使其與您[清單價格](./listing-price.md)中定義的&#x200B;_[!UICONTROL Magento Price Source]_不同。 若要根據您的_[!UICONTROL Magento Price Source]_&#x200B;設定調整您的刊登價格（向上或向下），請建立規則。 | [定價規則](./pricing-products.md) |

如需詳細資訊，請參閱[存放區設定](./ob-store-review.md)。
