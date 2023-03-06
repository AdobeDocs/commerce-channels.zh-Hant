---
title: 產品清單條件
description: 使用產品清單條件設定將您的商務產品對應至Amazon產品條件，例如「新」或「翻新」。
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 產品清單條件

產品清單條件設定是您商店清單設定的一部分。 您可以存取 [儲存儀表板](./amazon-store-dashboard.md).

Amazon需要產品清單才能有定義的條件。 如果您的所有產品都是相同的條件，您可以選取其中一個Amazon條件選項，將所有產品表示為全域條件值。 標準Amazon條件包括：

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
>如果您銷售續訂（翻新）的產品，則必須註冊 [!DNL Amazon Renewed Program]. 請參閱 [續訂產品](./renewed-products.md).

但是，如果目錄包含不同條件（如「新」、「已使用」和「已翻新」）的產品，則必須選擇 **[!UICONTROL Assign Condition Using Product Attribute]**. 此設定可讓您對應 [!DNL Commerce] 條件屬性和值，以取得Amazon清單的條件。

期間 [預先設定任務](./amazon-pre-setup-tasks.md)，您可以建立 [!DNL Commerce] 產品條件的產品屬性。 如果您提供不同條件的產品，但尚未建立條件屬性，請參閱 [在中建立產品屬性 [!DNL Commerce]](./ob-creating-magento-attributes.md). 建立條件屬性後，您可以為 [!DNL Commerce] 目錄。

## 配置設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店控制面板上。

1. 展開 **[!UICONTROL Product Listing Condition]** 區段。

1. 針對 **[!UICONTROL Listing Product Condition]**，選擇選項。

   為您所有清單的全域條件值，選擇其中一個標準Amazon條件。 預設設定為 `New`.

   如果您的產品/清單具有不同的條件，請選擇 `Assign Condition Using Product Attribute` 在顯示的其他欄位中定義產品條件設定。

1. 針對 **條件屬性**，選擇 [!DNL Commerce] 屬性來對應每個標準Amazon條件屬性的值。

   若您的產品位於 `Used` 或 `Collectible` 條件，但您無法進一步區分，您可以對應至單一 `Used` 或 `Collectible` Amazon條件，並將其他項目留空。 此方法會映射 `Used` 或 `Collectible` 條件轉換為單一Amazon已使用或可收集條件。

   例如，您有 `Used` 條件。 對應時，您可以選擇要對應至Amazon條件 `Used; Like New`, `Used; Very Good`, `Used; Good`，或 `Used; Acceptable`. 僅填妥您要的Amazon條件欄位，將另一個保留 `Used` 選項設定為 `--Select Option--`. 在範例影像中，全部 [!DNL Commerce] 產品 `Used` 條件已對應至Amazon `Used; Very Good` 條件。

   您也可以為條件輸入描述性文字，但 `New`.

1. 完成後，按一下 **[!UICONTROL Save listing settings]**.

![產品清單條件](assets/amazon-product-listing-condition.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Listing Product Condition] | 產品清單的條件。 選項： `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>如果您銷售單一產品條件，請選擇其中一個標準Amazon條件。 若您的 [!DNL Commerce] 目錄包含各種條件的產品，請選擇 `Assign Condition Using Product Attribute`. |
| [!UICONTROL Condition Attribute] | 此 [!DNL Commerce] 定義產品條件的屬性。 選取您建立的Magneto屬性，以對應至Amazon條件屬性。 在 [預先設定任務示例](./ob-creating-magento-attributes.md) 建議將命名為 `Amazon Condition`. 選取後，會顯示其他欄位以對應標準Amazon條件。 |
| [!UICONTROL Additional Condition fields] | 針對每個標準Amazon條件，選擇對應的條件。 選項是您在 [建立Amazon條件屬性](./ob-creating-magento-attributes.md).<br><br>若您的產品位於 `Used` 或 `Collectible` 條件，但您無法進一步區分，您可以對應至單一 `Used` 或 `Collectible` Amazon條件，並將其他項目留空。 此方法會映射所有 `Used` 或 `Collectible` 條件轉換為單一Amazon已使用或可收集條件。 |

**快速存取** - [!UICONTROL Listing Settings] 區段

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
