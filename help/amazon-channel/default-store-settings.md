---
title: 預設商店設定
description: 修改預設的商務設定，以自訂您商店的AmazonSales Channel。
exl-id: 368e5e8e-2bf9-4f9c-86c6-6d375f8a8720
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 預設商店設定

連線您的商店並設定第一個清單規則後，Amazon和 [!DNL Commerce] 開始。 存放區設定有數種類型，可讓您根據需求自訂存放區。 存取商店設定 [儀表板](./amazon-store-dashboard.md).

商店設定包括：

- [**[!UICONTROL Listing settings]**](./listing-settings.md)  — 控制產品目錄與 [!DNL Amazon Marketplace].

- [**[!UICONTROL Order settings]**](./order-settings.md)  — 控制Amazon訂單的管理方式。

- [**[!UICONTROL Listing rules]**](./listing-rules.md)  — 定義哪些目錄產品可列在Amazon上。

- [**[!UICONTROL Pricing rules]**](./pricing-products.md)  — 定義Amazon價目表價格如何針對合格清單進行變更。

- **[!UICONTROL Store reports]** - [競爭價格分析](./competitive-price-analysis.md) 和 [清單改進](./listing-improvements.md).

- **[!UICONTROL Logs]** - [列出變更](./listing-changes-log.md) 和 [通信錯誤](./communication-errors-log.md).

- [**[!UICONTROL Store integration settings]**](./store-integration-settings.md)  — 在 [!DNL Commerce] 管理員。

## 一些重要的預設設定

| 設定 | 預設 | 說明 | 位置 |
|--- |--- |--- |--- |
| [!UICONTROL Import Amazon Orders] | `Enabled` | 建立對應的 [!DNL Commerce] 從Amazon收到新訂單時的訂單，可在 [[!DNL Commerce] 訂購](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流程。 當 `Disabled`,Amazon會訂購匯入訂單資訊以供檢閱，但您必須在 [!DNL Amazon Seller Central] 帳戶。 | [順序設定](./order-settings.md) |
| [!UICONTROL Customer Creation] | `No Customer Creation (guest)` | 來自Amazon訂單的客戶資料不會匯入至 [!DNL Commerce] 資料庫。 匯入的Amazon訂單會以訪客結帳的形式處理。 如果您想要建置 [!DNL Commerce] 客戶資料庫，您應將此設定變更為 `Build New Customer Account`. | [順序設定](./order-settings.md) |
| [!UICONTROL Automatic List Action] | `Automatically List Eligible Products` | [!DNL Commerce] 目錄產品(符合Amazon的資格要求)以自動發佈至Amazon並建立Amazon清單。 如果您想要手動檢閱和發佈產品，應將此設定變更為 `Do Not Automatically List Eligible Products`. 等待手動發佈的產品會顯示在 [_準備列出_](./ready-to-list.md) 標籤。 | [產品清單動作](./product-listing-actions.md) |
| [!UICONTROL Magento Price Source] | `Price` | 定義價格來源屬性，作為Amazon清單的基礎。 如果您不想使用 [!DNL Commerce] `Price` 屬性作為定價規則所依據的基本價格，您應將此設定變更為其他屬性。 | [上市價](./listing-price.md) |
| [!UICONTROL Product Fulfilled By] | `Fulfilled by Merchant` | 商人履行了所有的命令。 如果您使用「由Amazon完成」或使用混合履行方法，則應變更此設定。 | [履行者](./listing-price.md) |
| [!UICONTROL Listing Product Condition] | `New` | 如果您的所有產品都是相同的條件，您可以選取其中一個Amazon條件選項來代表您的所有產品。 如果您的目錄包含不同條件（例如「新」、「已使用」和「已翻新」）的產品，您必須將此設定變更為 `Assign Condition Using Product Attribute` 將 [!DNL Commerce] 條件屬性至您的Amazon清單條件。 | [產品清單條件](./product-listing-condition.md) |
| [!UICONTROL Listing Rules] | 無 | 定義用於判斷哪些產品Amazon銷售管道會發佈至Amazon的規則。 這些規則提供許多選項，可建立簡單到複雜的規則，以將產品納入或排除為清單。 | [上市規則](./listing-rules.md) |
| 定價規則 | 無 | 定義與已定義的不同的Amazon清單價格屬性 _[!UICONTROL Magento Price Source]_在 [上市價](./listing-price.md). 根據您的_[!UICONTROL Magento Price Source]_ 設定，建立規則。 | [定價規則](./pricing-products.md) |

如需詳細資訊，請參閱 [商店設定](./ob-store-review.md).
