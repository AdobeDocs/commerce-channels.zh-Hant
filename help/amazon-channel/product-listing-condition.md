---
title: Amazon銷售管道 — 產品清單條件
description: 使用產品清單條件設定將您的Commerce產品對應至Amazon產品條件，例如「新增」或「整修」。
feature: Sales Channels, Products, Merchandising
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# 產品清單條件

產品清單條件設定是商店清單設定的一部分。 您可以存取清單上的清單設定， [存放區儀表板](./amazon-store-dashboard.md).

Amazon需要產品清單才能有定義的條件。 如果所有產品具有相同條件，您可以選取其中一個Amazon條件選項，將所有產品表示為您的全域條件值。 標準Amazon條件包括：

- `New`
- `Refurbished`
- `Used; Like New`
- `Used; Very Good`
- `Used; Good`
- `Used; Acceptable`
- `Collectible; Like New`
- `Collectible; Very Good`
- `Collectible; Good`
- `Collectible; Acceptable`

>[!IMPORTANT]
>
>如果您銷售更新（翻新）的產品，則必須註冊 [!DNL Amazon Renewed Program]. 另請參閱 [已續訂的產品](./renewed-products.md).

不過，如果您的目錄包含不同條件的產品（例如「新增」、「已使用」和「已翻新」），您必須選擇 **[!UICONTROL Assign Condition Using Product Attribute]**. 此設定可讓您對應 [!DNL Commerce] 條件屬性和值至您的Amazon清單條件。

期間 [預先設定任務](./amazon-pre-setup-tasks.md)，建議您建立 [!DNL Commerce] 產品條件的產品屬性。 如果您以各種條件提供產品，但尚未建立條件屬性，請參閱 [在中建立產品屬性 [!DNL Commerce]](./ob-creating-magento-attributes.md). 建立條件屬性後，您可將條件值指派給環境中的每項產品， [!DNL Commerce] 目錄。

## 設定設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店控制面板上。

1. 展開 **[!UICONTROL Product Listing Condition]** 區段。

1. 的 **[!UICONTROL Listing Product Condition]**，選擇一個選項。

   為所有清單的全域條件值選擇其中一個標準Amazon條件。 預設設定為 `New`.

   如果您的產品/清單具有不同的條件，請選擇 `Assign Condition Using Product Attribute` 在出現的其他欄位中定義產品條件設定。

1. 的 **條件屬性**，選擇 [!DNL Commerce] 屬性，對應每個標準Amazon條件屬性的值。

   如果您的產品在 `Used` 或 `Collectible` 條件，但若您不進一步區分，則可對應至單一 `Used` 或 `Collectible` Amazon條件，並將其他條件保留空白。 此方法會將您所有的 `Used` 或 `Collectible` 單一Amazon使用或可收集條件的條件。

   例如，您有一個 `Used` 產品的條件。 對應時，您可以選擇是否要對應至Amazon條件 `Used; Like New`， `Used; Very Good`， `Used; Good`，或 `Used; Acceptable`. 僅針對您想要的Amazon條件填寫欄位，留下其他 `Used` 選項已設定為 `--Select Option--`. 在範例影像中，所有 [!DNL Commerce] 中的產品 `Used` 條件對應至Amazon `Used; Very Good` 條件。

   您也可以輸入條件的描述性文字，但以下情況除外 `New`.

1. 完成後，按一下 **[!UICONTROL Save listing settings]**.

![產品清單條件](assets/amazon-product-listing-condition.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Listing Product Condition] | 產品清單的條件。 選項： `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>如果您銷售單一產品條件，請選擇其中一個標準Amazon條件。 若您的 [!DNL Commerce] 目錄包含各種狀況的產品，請選擇 `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | 此 [!DNL Commerce] 定義產品條件的屬性。 選取您建立的Magneto屬性，以對應至Amazon條件屬性。 在 [預先設定任務範例](./ob-creating-magento-attributes.md) 建議將其命名為 `Amazon Condition`. 選擇後，會出現其他欄位以對映標準Amazon條件。 |
| [!UICONTROL Additional Condition fields] | 針對每個標準Amazon條件，選擇對應的條件。 選項是您新增的條件標籤 [已建立您的Amazon條件屬性](./ob-creating-magento-attributes.md).<br><br>如果您的產品在 `Used` 或 `Collectible` 條件，但若您不進一步區分，則可對應至單一 `Used` 或 `Collectible` Amazon條件，並將其他條件保留空白。 此方法會對映所有 `Used` 或 `Collectible` 單一Amazon使用或可收集條件的條件。 |

**快速存取** - [!UICONTROL Listing Settings] 區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
