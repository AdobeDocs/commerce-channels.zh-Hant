---
title: 產品清單條件
description: 使用「產品清單條件」設定將您的Commerce產品映射到Amazon產品條件，如「新建」或「已翻新」。
redirect_from: /sales-channels/asc/ob-product-listing-condition.html
exl-id: f37ce3cf-7bfc-4dee-931e-a603008a71b8
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# 產品清單條件

產品清單條件設定是您的商店清單設定的一部分。 您可以訪問 [儲存儀表板](./amazon-store-dashboard.md)。

Amazon要求產品清單具有定義的條件。 如果您的所有產品都是相同的條件，則可以選擇一個Amazon條件選項來將您的所有產品表示為全局條件值。 標準Amazon條件包括：

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
>如果您銷售續訂（翻新）產品，則必須註冊 [!DNL Amazon Renewed Program]。 請參閱 [續訂的產品](./renewed-products.md)。

但是，如果目錄包含不同條件（如「新建」、「已用」和「已翻新」）的產品，則必須選擇 **[!UICONTROL Assign Condition Using Product Attribute]**。 此設定允許您映射 [!DNL Commerce] condition屬性和值到Amazon清單的條件。

期間 [預設定任務](./amazon-pre-setup-tasks.md)，鼓勵您建立 [!DNL Commerce] 產品狀況的product屬性。 如果您在各種條件下提供產品，但尚未建立條件屬性，請參閱 [在中建立產品屬性 [!DNL Commerce]](./ob-creating-magento-attributes.md)。 在建立條件屬性後，您可以將條件值分配給 [!DNL Commerce] 目錄。

## 配置設定

1. 按一下 **[!UICONTROL Listing Settings]** 在商店儀表板上。

1. 展開 **[!UICONTROL Product Listing Condition]** 的子菜單。

1. 對於 **[!UICONTROL Listing Product Condition]**，也請參見Wiki頁。

   為所有清單的全局條件值選擇一個標準Amazon條件。 預設設定為 `New`。

   如果您的產品/清單具有不同的條件，請選擇 `Assign Condition Using Product Attribute` 定義您的產品條件設定。

1. 對於 **條件屬性**&#x200B;的子菜單。 [!DNL Commerce] 屬性，以映射每個標準Amazon條件屬性的值。

   如果您在 `Used` 或 `Collectible` 條件，但你不能進一步區分，你可以映射到 `Used` 或 `Collectible` Amazon的情況，讓其他人不知道。 此方法映射所有 `Used` 或 `Collectible` 的Used或Colluble條件。

   例如，您有 `Used` 的下界。 映射時，您選擇是否要映射到Amazon條件 `Used; Like New`。 `Used; Very Good`。 `Used; Good`或 `Used; Acceptable`。 只填寫所需的Amazon條件欄位，將另一個 `Used` 選項設定為 `--Select Option--`。 在示例影像中，所有 [!DNL Commerce] 產品 `Used` 條件映射到Amazon `Used; Very Good` 的子菜單。

   您還可以輸入條件的描述性文本，但 `New`。

1. 完成後，按一下 **[!UICONTROL Save listing settings]**。

![產品清單條件](assets/amazon-product-listing-condition.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Listing Product Condition] | 產品清單的條件。 選項： `New` / `Refurbished` / `Used: Like New` / `Used: Very Good` / `Used: Good` / `Used: Acceptable` / `Collectible: Like New` / `Collectible: Very Good` / `Collectible: Good` / `Collectible: Acceptable` / `Assign Condition Using Product Attribute`<br><br>如果您銷售的是單一產品條件，請選擇標準Amazon條件之一。 如果 [!DNL Commerce] 目錄包含各種條件的產品，選擇 `Assign Condition Using Product Attribute`。 |
| [!UICONTROL Condition Attribute] | 的 [!DNL Commerce] 定義產品條件的屬性。 選擇您建立以映射到Amazon條件屬性的磁磁屬性。 在 [預設定任務示例](./ob-creating-magento-attributes.md) 建議將其命名為 `Amazon Condition`。 選中後，將顯示用於映射標準Amazon條件的附加欄位。 |
| [!UICONTROL Additional Condition fields] | 對於每個標準Amazon條件，選擇相應的條件。 這些選項是您在您 [建立了您的Amazon條件屬性](./ob-creating-magento-attributes.md)。<br><br>如果您在 `Used` 或 `Collectible` 條件，但你不能進一步區分，你可以映射到 `Used` 或 `Collectible` Amazon的情況，讓其他人不知道。 此方法映射所有 `Used` 或 `Collectible` 的Used或Colluble條件。 |

**快速訪問** - [!UICONTROL Listing Settings] 節

- [[!UICONTROL Product Listing Actions]](./product-listing-actions.md)
- [[!UICONTROL Third Party Listings]](./third-party-listing-settings.md)
- [[!UICONTROL Listing Price]](./listing-price.md)
- [[!UICONTROL (B2B) Business Price]](./business-pricing.md)
- [[!UICONTROL Stock / Quantity]](./stock-quantity.md)
- [[!UICONTROL Fulfilled By]](./fulfilled-by.md)
- [[!UICONTROL Catalog Search]](./catalog-search.md)
- [[!UICONTROL Product Listing Condition]](./product-listing-condition.md)
