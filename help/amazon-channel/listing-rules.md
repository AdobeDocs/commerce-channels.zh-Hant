---
title: Amazon銷售管道 — [!UICONTROL Listing Rules]
description: 使用清單規則可決定以Commerce Marketplace清單形式發佈的Amazon目錄產品。
feature: Sales Channels, Products
exl-id: b28a625b-64cf-4119-98bb-f1ea33043c8f
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# [!UICONTROL Listing Rules]

您可以存取[存放區儀表板](./amazon-store-dashboard.md)中存放區的清單規則。

清單規則定義規則，以判斷Amazon銷售管道會將哪些產品發佈至Amazon。 這些規則提供許多選項，可建立從簡單到複雜的規則，以將產品納入或排除為清單。 每個規則都包含設定產品清單資格要求的條件。

您的清單規則會持續與您的[!DNL Commerce]目錄同步。 當您新增符合清單規則所設定資格要求的新[!DNL Commerce]產品時，系統會自動處理這些產品以便將其列在Amazon上。

- 如果您希望將所有產品發佈至Amazon清單，請勿為清單規則定義任何條件。

- 如果您想要限制已發佈至Amazon的目錄產品，請定義清單規則條件。 定義Amazon清單規則的條件，會遵循定義[購物車價格規則](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html)條件的相同邏輯和程式。

- 如果您的清單規則排除產品，則該產品的資格狀態會變更為`Ineligible`。 不符合資格的產品不會發佈至Amazon。

- 如果不符合資格的產品已經列在Amazon上，並且您將Amazon清單與您的[!DNL Commerce]目錄產品相符，則Amazon清單的數量將變更為`0`以防止產品銷售。 Amazon清單可以[手動移除](./end-listings-manually.md)。

數量和資格狀態的變更會影響市集中針對相同地區商店銷售共用Amazon賣家SKU的所有清單（如[商店整合](./store-integration.md)期間&#x200B;_[!UICONTROL Amazon Marketplace Country]_中所定義）。 但是，變更一個地區的共用[!DNL Amazon Seller SKU]不會影響產品在不同國家/地區的Amazon清單。

![清單規則](assets/ob-listing-rules.png){width="600" zoomable="yes"}

## 設定清單規則設定

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Rules]**。

1. 定義您要在Amazon上列出之產品資格的條件。

請參閱[範例：定義條件](./ob-define-condition-example.md)。

| 欄位 | 說明 |
|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Websites] | 可用的選項取決於您在[!DNL Commerce]設定中設定的[網站](https://experienceleague.adobe.com/docs/commerce-admin/start/setup/websites-stores-views.html)。 針對Amazon上列出的合格產品選取網站。 您只能選取一個網站，因為每個網站都需要在Amazon銷售管道中建立唯一的Amazon商店。 |
| [!UICONTROL Conditions] | 用於定義[!DNL Commerce]屬性，以取得您Amazon地區的產品資格。 請參閱[範例：定義條件](./ob-define-condition-example.md)。 |

## 條件工作區

條件中任何粗體的區域都可以按一下，以檢視各種選項。

- 如果所選網站內的所有產品都合格，請勿新增條件。
- 要直接與Amazon的系統通訊，有一組複雜的後端程式。 根據您嘗試列出的專案數量，以及Amazon的系統可能有多忙（例如「黑色星期五」），您的專案可能需要一些時間才會列在Amazon上。

如需條件的詳細資訊，請參閱[描述條件](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html)。

## 清單規則預覽

當您修改清單規則的條件定義時，可以按一下&#x200B;**[!UICONTROL Preview Changes]**&#x200B;套用規則變更，並檢視清單如何受到影響。 儲存清單規則變更之前，請先在此清單預覽功能中驗證您的清單。

您的Amazon清單會與規則和定義的條件做比較。 然後您可以檢閱：

- 根據您目前的[!DNL Amazon Seller Central]帳戶，哪些產品會移至不合格狀態
- 哪些產品會從不符合資格狀態移回符合資格狀態
- 哪些產品是新的Amazon清單，並從符合資格的[!DNL Commerce]產品新增至您的Amazon清單

清單預覽可讓您預覽潛在的Amazon清單，並對清單規則進行任何必要的調整。

您的潛在Amazon清單會在&#x200B;_[!UICONTROL Listing Preview]_頁面上填入三個索引標籤之一：

- **[!UICONTROL Ineligible Listings]** — 根據您目前的清單規則與條件，列出的產品不符合Amazon清單的資格。

  不符合資格的產品不會發佈至Amazon。 如果不符合資格的產品已經列在Amazon上，並且您將Amazon清單與您的[!DNL Commerce]目錄產品相符，則Amazon清單的數量將變更為`0`以防止產品銷售。 若要手動移除清單，請參閱[結束Amazon清單](./end-listings-manually.md) 不符合Amazon要求的產品在此不列出。 這些產品列在[非使用中清單索引標籤](./inactive-listings.md)上。

- **[!UICONTROL Eligible Listings]** — 根據您目前的清單規則與條件，列出的產品符合Amazon清單資格，也符合Amazon要求。 此清單包含您匯入的現有Amazon清單（如果您在[清單設定](./third-party-listing-settings.md)中將&#x200B;**匯入協力廠商清單**&#x200B;設定為`Import Listing`）。

- **[!UICONTROL New Listings]** — 列出的產品包含您的[!DNL Commerce]目錄產品，這些產品是根據您目前的清單規則和條件新符合Amazon清單資格，並且建立和發佈新的Amazon清單。

### 檢視您的清單預覽

1. 按一下商店儀表板上的&#x200B;**[!UICONTROL Listing Rules]**。

1. 檢視或新增您的[清單規則](./listing-rules.md)。

1. 修改您的[清單規則條件](./ob-define-condition-example.md)。

1. 按一下&#x200B;**[!UICONTROL Preview Changes]**。

1. 檢閱並確認您在&#x200B;_[!UICONTROL Ineligible Listings]_、_[!UICONTROL Eligible Listings]_&#x200B;和&#x200B;_[!UICONTROL New Listings]_索引標籤中的清單。

1. 如果清單符合您的預期，請按一下&#x200B;**[!UICONTROL Save and close]**。

   如果您的清單未如預期顯示，請按一下&#x200B;**[!UICONTROL Back]**&#x200B;並修改您的規則和條件，直到清單符合您的預期為止。

![清單規則預覽](assets/amazon-listing-rule-preview.png){width="600" zoomable="yes"}

### 列出預覽記錄

| 欄位 | 說明 |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Product ID] | 在新增[!DNL Commerce]目錄產品時指派給該產品的不重複、連續編號。 |
| [!UICONTROL Thumbnail] | 顯示主要產品影像的縮圖。 |
| [!UICONTROL Name] | 在[!DNL Commerce] [產品網格](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/products-list.html)中管理的產品名稱。 |
| [!UICONTROL Type] | 在[!DNL Commerce]產品格線中管理的產品型別。 |
| [!UICONTROL Attribute Set] | 在[!DNL Commerce]產品格線中管理的用作產品範本的屬性集名稱。 |
| [!UICONTROL SKU] | 指派給產品的唯一庫存單位，在[!DNL Commerce]產品格線中管理。 |
| [!UICONTROL Visibility] | 表示產品在[!DNL Commerce]產品格線中的可見位置。 選項：<ul><li>`Not visible individually`</li><li>`Catalog`</li><li>`Search`</li><li>`Catalog, Search`</li></ul> |
| 狀態 | 表示在[!DNL Commerce]產品格線中管理的產品狀態。 選項： `Enabled` / `Disabled` |

![正在列出預覽工作流程](assets/listing-preview-flowchart.png){width="500" zoomable="yes"}
