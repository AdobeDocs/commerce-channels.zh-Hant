---
title: '''示例：定義條件」'
description: 在建立上市規則時，定義用於標識要在Amazon市場上列出的Commerce目錄產品的條件。
exl-id: 8a48acfc-d31b-4919-bef7-8c300f0f9d94
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---

# 示例：定義條件

## 條件

可以按一下條件中任何粗體區域以查看各種選項。

**如果所選網站中的所有產品均符合條件，則不要添加條件。**

>[!NOTE]
>
>有一套複雜的後端流程可以直接與Amazon的系統通信。 根據您嘗試列出的項目數以及Amazon系統可能有多忙（如「黑色星期五」），您的項目可能需要時間才能在Amazon列出。

請參閱的「條件」部分 [建立購物車價格規則](https://docs.magento.com/user-guide/marketing/price-rules-catalog-create.html){target="_blank"}。

## 定義條件

此過程可以是簡單的，也可以是詳細的，具體取決於您的目錄設定。 你可以設定條件，這樣 `ALL` 或 `ANY` 定義條件 `TRUE` 或 `FALSE` 產品，則產品有資格在Amazon上市。

條件基於現有產品屬性值。 要將規則應用於所有產品，請將條件部分留空。

>[!NOTE]
>
>如果要基於特定產品屬性定義條件，請設定 **[!UICONTROL Use for Promo Rule Conditions]** 將屬性設定為 `Yes`。 您可以在 [店面屬性](https://docs.magento.com/user-guide/catalog/product-attributes-add.html){target="_blank"} 的子菜單。

![條件 — 行1](assets/ob-listing-rule-conditions-start.png)

此示例中的規則定義一個規則，該規則為具有以下條件的所有目錄產品設定Amazon資格： _AmazonFBA_ 屬性集 `Yes`。

規則語句有兩個粗體連結，按一下後，這些連結將顯示該語句部分的選項。 如果保存條件而不更改粗體選項，則該規則適用於所有產品。

- 按一下 **[!UICONTROL ALL]** 選擇 `ALL` 或 `ANY`。
- 按一下 **[!UICONTROL TRUE]** 選擇 `TRUE` 或 `FALSE`。
- 要將規則應用於所有產品，請保持條件不變。

可以通過更改這些值的組合來建立不同的條件。 在此示例中，使用以下條件：

`If ALL of these conditions are TRUE:`

1. 按一下添加(![添加表徵圖](assets/btn-add-grn.png))表徵圖，並選擇要作為條件基礎的屬性，如條件組合或產品屬性。

   - **[!UICONTROL Conditions Combination]**  — 選擇允許您建立另一組 `All/Any` 和 `True/False` 現有集內的條件。

      ![條件組合](assets/ob-conditions-combinations.png)

   - **[!UICONTROL Product Attribute]**  — 產品屬性取決於屬性的設定。 要使屬性顯示在清單中，必須為在提升規則條件中的使用配置屬性。 查看 _用於促銷規則條件_ 在 [產品屬性](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"}。

      在 **[!UICONTROL Product Attribute]**，選擇要用作條件基礎的屬性。 對於此示例，所選條件為 `Amazon FBA`。

      ![條件行2，第2部分](assets/ob-condition-attribute-dropdown.png)

      所選條件出現在語句中，然後是兩個更粗體的連結。 這些選項因您選擇的產品屬性而異。

      設定該屬性後，將無法更改。 要更改屬性，必須刪除行並添加新屬性。 通過按一下刪除(![刪除表徵圖](assets/btn-del-red.png))表徵圖。

      1. 按一下 **[!UICONTROL is]** 並選擇描述產品滿足條件的比較運算子。

         對於本示例，比較運算子為 `is`。 可用選項取決於在上一步中選擇的屬性。 選項可以包括不同的比較選項，例如匹配值，不包括或包括值中的至少一個值，並且大於、等於和小於數值。 在此示例中，選項為 `is` 和 `is not`。

      1. 按一下 **[!UICONTROL ...]** 並選擇條件所基於的屬性值。

         這些選項取決於屬性的設定。 系統可能會提示您選擇一個選項，或輸入條件的文本或數值。 對於此示例，選擇 `Yes`。

         所選項將出現在語句中以完成條件。

         ![條件行2，第3部分](assets/ob-listing-rule-condition-is.png)
   此條件已完成。 如前所述，此條件表示 [!DNL Commerce] 將AmazonFBA屬性設定為值的目錄 `Yes` 有資格在Amazon上市，供該地區及店鋪使用。 您可以添加更多條件行，以進一步縮小合格產品的範圍。

1，要向語句添加另一個條件行，請返回到步驟1並重複該過程，直到所有所需條件都完成。

通過按一下刪除(![刪除表徵圖](assets/btn-del-red.png))表徵圖。
