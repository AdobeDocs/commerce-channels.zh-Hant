---
title: 價格規則條件
description: 使用價格規則條件來確定哪些產品符合上市價格規則的條件。
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: ac190d88711f07c0b255a8cb50b12b62945f625e
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# 價格規則條件

條件決定哪些產品符合價格規則。 定義Amazon定價規則的條件時遵循的邏輯和程式與定義[!DNL Commerce]中[購物車價格規則](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){:target=&quot;_blank&quot;}的條件相同。

>[!IMPORTANT]
>
>如果您的價格規則適用於[!DNL Commerce]目錄中的所有產品，請將此區段留空。

條件中任何粗體的區域都可點選，以查看各種選項。

## 範例：建立價格規則條件

此程式可能簡單或詳細，視您的目錄設定而定。 您可以定義條件，以便當條件的`ALL`或`ANY`對於產品為`TRUE`或`FALSE`時，產品符合要套用的定價規則的資格。

條件是以您的[產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}為基礎。 若要將規則套用至所有產品，請將條件區段保留空白。

>[!NOTE]
>
>如果要根據特定產品屬性定義條件，則屬性的&#x200B;**使用促銷規則條件**&#x200B;必須在屬性的[Storefront屬性](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}中設定為`Yes`。

![價格規則條件 — 第1行](assets/ob-price-rules-condition-1.png)

此示例定義一個規則，該規則對`Books`類別中定義的所有產品應用25%折扣。

規則陳述式有兩個粗體連結，按一下後，這些連結會顯示condition陳述式中該部分的選項。 如果您儲存條件而未變更粗體選項，規則會套用至所有產品。

- 按一下&#x200B;**[!UICONTROL ALL]**，然後選擇`ALL`或`ANY`。
- 按一下&#x200B;**[!UICONTROL TRUE]**，然後選擇`TRUE`或`FALSE`。
- 若要將規則套用至所有產品，請維持條件不變。

您可以變更這些值的組合，以建立不同的條件。 在此範例中，會使用下列條件：

`If ALL of these conditions are TRUE:`

1. 若要顯示條件要套用的可用屬性，請按一下條件行開頭的「添加」（![添加表徵圖](assets/btn-add-grn.png)）表徵圖，並選擇一個屬性作為條件的基礎。

   **[!UICONTROL Conditions Combination]**  — 選擇在現有條件內 `All/Any` 建 `True/False` 立另一組和條件。

   ![價格規則條件組合](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]**  — 可用的產品屬性取 [決於屬性](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}的設定。若要讓清單中顯示的屬性，您的[storefront屬性](https://docs.magento.com/user-guide/stores/attribute-product-create.html){:target=&quot;_blank&quot;}中，屬性的&#x200B;*[!UICONTROL Use for Promo Rule Conditions]*&#x200B;必須設為`Yes`。

   - 對於&#x200B;**[!UICONTROL Product Attribute]**，選擇要定義為條件基礎的屬性。 在此範例中，選取的條件為`Category`。

      ![價格規則條件 — 第2行，第2部分](assets/ob-price-rule-condition-2.png)

      選取的條件會出現在陳述式中，後面接著兩個粗體連結。 選項會依您選取的產品屬性而有所不同。

      設定屬性後，就無法編輯該屬性。 若要變更屬性，您必須刪除該行並新增新屬性。 您可以按一下條件行結尾的「刪除」(![刪除」圖示](assets/btn-del-red.png)圖示，以刪除條件行。

   - 按一下&#x200B;**[!UICONTROL is]**&#x200B;並選擇描述產品要滿足條件的比較運算子。

      在此範例中，比較運算子為`is`。 可用選項取決於上一步中選取的屬性，並可能包含不同的比較選項。 選項可以包括匹配值，不包括或包括值中的至少一個，以及大於、等於和小於數值量。 在此範例中，選項為`is`和`is not`。

   - 按一下&#x200B;**[!UICONTROL ...]**&#x200B;並選擇條件所依據的屬性值。 選項取決於屬性的設定。

      系統可能會提示您選取選項或輸入條件的值。 在此範例中，欄位顯示為空白。 若要為規則選擇類別，請按一下選擇器表徵圖（![選擇器表徵圖](assets/btn-chooser.png)）以顯示您的選擇選項。 此規則適用於&#x200B;_Books_，選中&#x200B;**[!UICONTROL Books]**&#x200B;複選框。 類別編號會填入。 要接受類別選擇，請按一下綠色複選標籤表徵圖（![複選標籤表徵圖](assets/btn-check-mark-green.png)）。

      ![價格規則條件 — 第2行，第3部分](assets/ob-price-rule-condition-3.png)

      所選項將出現在語句中以完成條件。

      ![價格規則條件 — 第2行，第4部分](assets/ob-price-rule-condition-4.png)

      此範例條件已完成。 如前所述，此條件表示[!DNL Commerce]目錄中具有已定義帳簿類別(`4`)的任何產品均符合此定價規則。 您可以新增更多條件行，進一步縮小符合條件的產品。

1. 若要將其他條件行新增至陳述式，請返回步驟1並重複此程式，直到所有需要的條件完成為止。

   您隨時可以按一下條件陳述式結尾的「刪除」（![Delete圖示](assets/btn-del-red.png)）圖示來刪除該條件陳述式的一行。
