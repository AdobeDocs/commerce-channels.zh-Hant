---
title: 價格規則條件
description: 使用價格規則條件確定哪些產品符合上市價格規則的要求。
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# 價格規則條件

條件確定哪些產品符合價格規則。 為Amazon定價規則定義條件遵循與定義條件相同的邏輯和流程 [購物車價格規則](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target="_blank"} 在 [!DNL Commerce]。

>[!IMPORTANT]
>
>如果價格規則適用於您的 [!DNL Commerce] 目錄，然後將此部分留空。

可以按一下條件中任何粗體區域以查看各種選項。

## 示例：建立價格規則條件

此過程可以是簡單的或詳細的，具體取決於您的目錄配置。 您可以定義條件，以便 `ALL` 或 `ANY` 條件是 `TRUE` 或 `FALSE` 對於產品，則產品有資格應用定價規則。

條件基於您 [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}。 要將規則應用於所有產品，請將條件部分留空。

>[!NOTE]
>
>如果要基於特定產品屬性定義條件， **用於促銷規則條件** 屬性必須設定為 `Yes` 在 [店面屬性](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target="_blank"} 的子菜單。

![價格規則條件 — 行1](assets/ob-price-rules-condition-1.png)

此示例定義一個規則，該規則對在 `Books` 的子菜單。

規則語句有兩個粗體連結，按一下這些連結時，將顯示該條件語句部分的選項。 如果保存條件而不更改粗體選項，則該規則適用於所有產品。

- 按一下 **[!UICONTROL ALL]** 選擇 `ALL` 或 `ANY`。
- 按一下 **[!UICONTROL TRUE]**，選擇 `TRUE` 或 `FALSE`。
- 要將規則應用於所有產品，請保持條件不變。

可以通過更改這些值的組合來建立不同的條件。 在此示例中，使用以下條件：

`If ALL of these conditions are TRUE:`

1. 要顯示條件適用的可用屬性，請按一下添加(![添加表徵圖](assets/btn-add-grn.png))表徵圖，並選擇要作為條件基礎的屬性。

   **[!UICONTROL Conditions Combination]**  — 選擇建立另一組 `All/Any` 和 `True/False` 條件。

   ![價格規則條件組合](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]**  — 可用產品屬性取決於 [屬性的設定](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target="_blank"}. For an attribute to show in the list, *[!UICONTROL Use for Promo Rule Conditions]* for the attribute must be set to `Yes` in your [storefront properties](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target="_blank"}。

   - 對於 **[!UICONTROL Product Attribute]**，選擇要定義為條件基礎的屬性。 對於此示例，所選條件為 `Category`。

      ![價格規則條件 — 第2行，第2部分](assets/ob-price-rule-condition-2.png)

      所選條件出現在語句中，然後是兩個更粗體的連結。 這些選項因您選擇的產品屬性而異。

      設定該屬性後，將無法對其進行編輯。 要更改屬性，必須刪除行並添加新屬性。 通過按一下刪除(![刪除表徵圖](assets/btn-del-red.png) 表徵圖。

   - 按一下 **[!UICONTROL is]** 並選擇描述產品滿足條件的比較運算子。

      對於本示例，比較運算子為 `is`。 可用選項取決於在上一步中選擇的屬性，並可能包含不同的比較選項。 選項可以包括匹配值，但不包括或包括值中的至少一個值，並且大於、等於和小於數值。 在此示例中，選項為 `is` 和 `is not`。

   - 按一下 **[!UICONTROL ...]** 並選擇條件所基於的屬性值。 這些選項取決於屬性的設定。

      可能會提示您選擇選項或輸入條件的值。 對於此示例，該欄位將顯示為空。 要為規則選擇類別，請按一下選擇器表徵圖(![選擇器表徵圖](assets/btn-chooser.png))顯示選擇選項。 此規則是 _書籍_，選擇 **[!UICONTROL Books]** 複選框。 將填充類別編號。 要接受類別選擇，請按一下綠色複選標籤表徵圖(![複選標籤表徵圖](assets/btn-check-mark-green.png))。

      ![價格規則條件 — 第2行，第3部分](assets/ob-price-rule-condition-3.png)

      所選項將出現在語句中以完成條件。

      ![價格規則條件 — 第2行，第4部分](assets/ob-price-rule-condition-4.png)

      此示例條件已完成。 如前所述，此條件表示 [!DNL Commerce] 具有已定義的帳簿類別的目錄(`4`)符合此定價規則。 您可以添加更多條件行，以進一步縮小合格產品的範圍。

1. 要向語句添加另一個條件行，請返回到步驟1並重複該過程，直到所有所需條件都完成。

   通過按一下刪除(![刪除表徵圖](assets/btn-del-red.png))表徵圖。
