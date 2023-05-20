---
title: 上市規則
description: 使用上市規則可確定作為Amazon市場清單發佈的Commerce目錄產品。
redirect_from: /sales-channels/asc/ob-listing-rules.html/sales-channels/asc/ob-listing-preview.html/sales-channels/asc/listing-rule-preview.html
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# 上市規則

您可以訪問儲存在 [儲存儀表板](./amazon-store-dashboard.md)。

上市規則界定規則，以決定Amazon銷售渠道向Amazon發佈哪些產品。 這些規則提供了許多選項來建立簡單到複雜的規則，以將產品作為清單包括或排除。 每個規則都包括設定產品清單資格要求的條件。

您的上市規則將與您的 [!DNL Commerce] 目錄。 添加新 [!DNL Commerce] 符合您的上市規則規定的資格要求的產品，產品將自動處理以在Amazon上市。

- 如果您希望所有產品都發佈到Amazon上市，請不要為您的上市規則定義任何條件。

- 如果要限制發佈到Amazon的目錄產品，請定義清單規則條件。 為Amazon上市規則定義條件遵循與定義以下條件相同的邏輯和流程 [購物車價格規則](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target="_blank"}。

- 如果您的上市規則排除了產品，則該產品的資格狀態將更改為 `Ineligible`。 不合格產品不發佈給Amazon。

- 如果Amazon上已列出不合格產品，並且您將Amazon清單與 [!DNL Commerce] 目錄產品，Amazon清單的數量更改 `0` 防止產品銷售。 Amazon清單 [已刪除](./end-listings-manually.md)。

數量和資格狀態的更改會影響為同一區域中的商店銷售而存在的市場中共用Amazon銷售商SKU的所有清單(定義如 _[!UICONTROL Amazon Marketplace Country]_在 [儲存整合](./store-integration.md))。 但是，對共用的更改 [!DNL Amazon Seller SKU] 在一個地區，該產品不會影響其在另一個國家的Amazon上市。

![上市規則](assets/ob-listing-rules.png)

## 配置清單規則設定

1. 按一下 **[!UICONTROL Listing Rules]** 在商店儀表板上。

1. 為要在Amazon列出的產品的資格定義所需條件。

請參閱 [示例：定義條件](./ob-define-condition-example.md)。

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Websites] | 可用選項取決於 [網站](https://docs.magento.com/user-guide/stores/websites-stores-views.html){target="_blank"} 你在 [!DNL Commerce] 配置。 為Amazon上列出的合格產品選擇網站。 只能選擇一個網站，因為每個網站都需要在Amazon銷售渠道中建立一個獨特的Amazon商店。 |
| [!UICONTROL Conditions] | 用於定義 [!DNL Commerce] 您的Amazon地區內產品資格的屬性。 請參閱 [示例：定義條件](./ob-define-condition-example.md)。 |

## 條件工作區

可以按一下條件中任何粗體區域以查看各種選項。

- 如果所選網站中的所有產品均符合條件，則不要添加條件。
- 有一套複雜的後端流程可以直接與Amazon的系統通信。 根據您嘗試列出的項目數以及Amazon系統可能有多忙（如「黑色星期五」），您的項目可能需要時間才能在Amazon列出。

有關條件的詳細資訊，請參見 [描述條件](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target="_blank"}。

## 清單規則預覽

修改上市規則的條件定義時，可按一下 **[!UICONTROL Preview Changes]** 應用規則更改並查看清單受到的影響。 在保存清單規則更改之前，請在此清單預覽功能中驗證您的清單。

您的Amazon清單將與您的規則和定義條件進行比較。 然後，您可以查看：

- 哪些產品將根據您當前的產品移動到不合格狀態 [!DNL Amazon Seller Central] 帳戶
- 哪些產品從不合格狀態移回合格狀態
- 哪些產品是新Amazon清單，並從您的合格產品添加到您的Amazon清單 [!DNL Commerce] 產品

「清單預覽」允許您預覽潛在的Amazon清單，並對清單規則進行任何必要的調整。

您的潛在Amazon清單填充在 _[!UICONTROL Listing Preview]_的下一頁。

- **[!UICONTROL Ineligible Listings]**  — 根據您當前的上市規則及條件，所列產品不符合Amazon上市資格。

   不合格產品不發佈給Amazon。 如果Amazon上已列出不合格產品，並且您將Amazon清單與 [!DNL Commerce] 目錄產品，Amazon清單的數量更改 `0` 防止產品銷售。 要手動刪除清單，請參閱 [結束Amazon上市](./end-listings-manually.md)。 不符合Amazon要求的產品不在此列出。 這些產品列在 [「非活動清單」頁籤](./inactive-listings.md)。

- **[!UICONTROL Eligible Listings]**  — 根據您當前的上市規則及條件，所列產品符合Amazon上市資格，並符合Amazon規定。 此清單包括導入的現有Amazon清單(如果 **導入第三方清單** 設定為 `Import Listing` 在 [列出設定](./third-party-listing-settings.md))。

- **[!UICONTROL New Listings]**  — 列出的產品包括 [!DNL Commerce] 根據您當前的上市規則和條件，對新有資格進入Amazon上市的產品進行編目，並建立和發佈新的Amazon上市。

### 查看清單預覽

1. 按一下 **[!UICONTROL Listing Rules]** 在商店儀表板上。

1. 查看或添加 [上市規則](./listing-rules.md)。

1. 修改 [清單規則條件](./ob-define-condition-example.md)。

1. 按一下 **[!UICONTROL Preview Changes]**。

1. 查看並確認您在 _[!UICONTROL Ineligible Listings]_。_[!UICONTROL Eligible Listings]_, _[!UICONTROL New Listings]_頁籤。

1. 如果您的清單符合您的期望，請按一下 **[!UICONTROL Save and close]**。

   如果您的清單未按預期顯示，請按一下 **[!UICONTROL Back]** 並修改您的規則和條件，直到您的清單符合您的期望。

![清單規則預覽](assets/amazon-listing-rule-preview.png)

### 列出預覽記錄

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Product ID] | 分配給的唯一、連續編號 [!DNL Commerce] 添加產品時編錄產品。 |
| [!UICONTROL Thumbnail] | 顯示主產品影像的縮略圖。 |
| [!UICONTROL Name] | 產品的名稱，在 [!DNL Commerce] [產品網格](https://docs.magento.com/user-guide/catalog/products.html){target="_blank"}。 |
| [!UICONTROL Type] | 產品類型，在 [!DNL Commerce] 產品網格。 |
| [!UICONTROL Attribute Set] | 用作產品模板的屬性集的名稱，在 [!DNL Commerce] 產品網格。 |
| [!UICONTROL SKU] | 分配給產品的唯一庫存單位，在 [!DNL Commerce] 產品網格。 |
| [!UICONTROL Visibility] | 指示產品在中的可見、管理的位置 [!DNL Commerce] 產品網格。 選項：<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| 狀態 | 指示產品的狀態，在 [!DNL Commerce] 產品網格。 選項： `Enabled` / `Disabled` |

![列出預覽工作流](assets/listing-preview-flowchart.png)
