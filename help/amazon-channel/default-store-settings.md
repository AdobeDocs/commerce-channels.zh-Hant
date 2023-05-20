---
title: 預設儲存設定
description: 修改預設的Commerce設定，以自定義您商店的AmazonSales Channel。
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 預設儲存設定

在您的商店連接並設定了第一個清單規則後，Amazon和 [!DNL Commerce] 開始。 存在幾種類型的儲存設定，允許您根據需要自定義儲存。 在儲存上訪問儲存設定 [儀表板](./amazon-store-dashboard.md)。

儲存設定包括：

- [**[!UICONTROL Listing settings]**](./listing-settings.md)  — 控制產品目錄與 [!DNL Amazon Marketplace]。

- [**[!UICONTROL Order settings]**](./order-settings.md)  — 控制管理Amazon訂單的方式。

- [**[!UICONTROL Listing rules]**](./listing-rules.md)  — 定義哪些目錄產品有資格在Amazon上列出。

- [**[!UICONTROL Pricing rules]**](./pricing-products.md)  — 定義如何更改符合條件的清單的Amazon價目表價格。

- **[!UICONTROL Store reports]** - [競爭價格分析](./competitive-price-analysis.md) 和 [清單改進](./listing-improvements.md)。

- **[!UICONTROL Logs]** - [列出更改](./listing-changes-log.md) 和 [通信錯誤](./communication-errors-log.md)。

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md)  — 查看以下位置的電子郵件和Amazon銷售渠道商店名稱設定： [!DNL Commerce] 管理員。

## 某些重要的預設設定

| 設定 | 預設 | 說明 | 位置 |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | 建立相應 [!DNL Commerce] 從Amazon接到新訂單時發出訂單，允許在 [[!DNL Commerce] 訂單](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流。 當 `Disabled`,Amazon訂單導入訂單資訊以供審閱，但您必須在您的訂單中管理訂單 [!DNL Amazon Seller Central] 帳戶。 | [訂單設定](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | 未將來自Amazon訂單的客戶資料導入您的 [!DNL Commerce] 資料庫。 導入的Amazon訂單作為來賓結帳處理。 如果你想要 [!DNL Commerce] customer資料庫，您應將此設定更改為 `Build New Customer Account`。 | [訂單設定](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] 目錄產品(符合Amazon的資格要求)自動發佈到Amazon並建立Amazon清單。 如果要手動審閱和發佈產品，應將此設定更改為 `Do Not Automatically List Eligible Products`。 等待手動發佈的產品將出現在 [_準備列出_](./ready-to-list.md) 頁籤。 | [產品清單操作](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | 定義用作您的Amazon清單基礎的價格來源屬性。 如果您不想使用 [!DNL Commerce] `Price` 屬性作為定價規則所依據的基本價格，您應將此設定更改為其他屬性。 | [上市價格](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | 商人履行所有訂單。 如果您使用Amazon的履行或使用多種履行方法，則應更改此設定。 | [履行者](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | 如果您的所有產品都是相同的條件，則可以選擇一個Amazon條件選項來表示您的所有產品。 如果目錄包含不同條件（如「新建」、「已用」和「已翻新」）的產品，則必須將此設定更改為 `Assign Condition Using Product Attribute` 映射 [!DNL Commerce] 條件屬性。 | [產品清單條件](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | 無 | 定義用於確定Amazon銷售渠道發佈到Amazon的產品的規則。 這些規則提供了許多選項來建立簡單到複雜的規則，以將產品作為清單包括或排除。 | [上市規則](./listing-rules.md) |
| 定價規則 | 無 | 定義與定義的價格不同的Amazon清單價格屬性 _[!UICONTROL Magento Price Source]_在 [上市價格](./listing-price.md)。 根據您的_[!UICONTROL Magento Price Source]_ 建立規則。 | [定價規則](./pricing-products.md) |

有關詳細資訊，請參見 [儲存設定](./ob-store-review.md)。
