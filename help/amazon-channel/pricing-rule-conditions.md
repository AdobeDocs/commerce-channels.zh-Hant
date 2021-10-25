---
title: 價格規則條件
description: 使用價格規則條件來確定哪些產品符合上市價格規則的條件。
redirect_from: /sales-channels/asc/ob-pricing-rules-conditions.html
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 15b9468d090b6ee79fd91c729f2481296e98c93a
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# 價格規則條件

條件決定哪些產品符合價格規則。 定義Amazon定價規則的條件時，遵循的邏輯和程式與定義 [購物車價格規則](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;} [!DNL Commerce].

>[!IMPORTANT]
>
>如果價格規則適用於 [!DNL Commerce] 目錄，然後將此區段保留空白。

條件中任何粗體的區域都可點選，以查看各種選項。

## 範例：建立價格規則條件

此程式可能簡單或詳細，視您的目錄設定而定。 您可以定義條件，以便 `ALL` 或 `ANY` 條件中， `TRUE` 或 `FALSE` 若是產品，則產品符合套用定價規則的資格。

條件以 [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}。 若要將規則套用至所有產品，請將條件區段保留空白。

>[!NOTE]
>
>如果您想根據特定產品屬性定義條件， **用於促銷規則條件** 屬性必須設為 `Yes` 在 [店面屬性](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}取得。

![價格規則條件 — 第1行](assets/ob-price-rules-condition-1.png)

此範例定義的規則會將25%折扣套用至 `Books` 類別。

規則陳述式有兩個粗體連結，按一下後，這些連結會顯示condition陳述式中該部分的選項。 如果您儲存條件而未變更粗體選項，規則會套用至所有產品。

- 按一下 **[!UICONTROL ALL]** 選擇 `ALL` 或 `ANY`.
- 按一下 **[!UICONTROL TRUE]**，選擇 `TRUE` 或 `FALSE`.
- 若要將規則套用至所有產品，請維持條件不變。

您可以變更這些值的組合，以建立不同的條件。 在此範例中，會使用下列條件：

`If ALL of these conditions are TRUE:`

1. 若要顯示條件要套用的可用屬性，請按一下新增(![新增圖示](assets/btn-add-grn.png))圖示，並選取要依據條件的屬性。

   **[!UICONTROL Conditions Combination]**  — 選擇建立另一組 `All/Any` 和 `True/False` 條件。

   ![價格規則條件組合](assets/ob-conditions-combinations.png)

   **[!UICONTROL Product Attribute]**  — 可用的產品屬性取決於 [屬性的設定](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}。 若要讓屬性顯示在清單中， *[!UICONTROL Use for Promo Rule Conditions]* 屬性必須設為 `Yes` 在 [店面屬性](https://docs.magento.com/user-guide/stores/attribute-product-create.html){target=&quot;_blank&quot;}。

   - 針對 **[!UICONTROL Product Attribute]**，選擇要定義為條件基礎的屬性。 在此範例中，選取的條件為 `Category`.

      ![價格規則條件 — 第2行，第2部分](assets/ob-price-rule-condition-2.png)

      選取的條件會出現在陳述式中，後面接著兩個粗體連結。 選項會依您選取的產品屬性而有所不同。

      設定屬性後，就無法編輯該屬性。 若要變更屬性，您必須刪除該行並新增新屬性。 您可以按一下「刪除」(![刪除圖示](assets/btn-del-red.png) 表徵圖。

   - 按一下 **[!UICONTROL is]** 並選擇描述產品滿足條件的比較運算子。

      在此範例中，比較運算子為 `is`. 可用選項取決於上一步中選取的屬性，並可能包含不同的比較選項。 選項可以包括匹配值，不包括或包括值中的至少一個，以及大於、等於和小於數值量。 在此範例中，選項為 `is` 和 `is not`.

   - 按一下 **[!UICONTROL ...]** 並選擇條件所依據的屬性值。 選項取決於屬性的設定。

      系統可能會提示您選取選項或輸入條件的值。 在此範例中，欄位顯示為空白。 若要選取規則的類別，請按一下選擇器圖示(![選擇器表徵圖](assets/btn-chooser.png))以顯示您的選取選項。 此規則適用於 _書籍_，請選取 **[!UICONTROL Books]** 核取方塊。 類別編號會填入。 若要接受類別選取，請按一下綠色勾號圖示(![勾號圖示](assets/btn-check-mark-green.png))。

      ![價格規則條件 — 第2行，第3部分](assets/ob-price-rule-condition-3.png)

      所選項將出現在語句中以完成條件。

      ![價格規則條件 — 第2行，第4部分](assets/ob-price-rule-condition-4.png)

      此範例條件已完成。 如上所述，此條件表示 [!DNL Commerce] 具有已定義的書類(`4`)符合此定價規則的資格。 您可以新增更多條件行，進一步縮小符合條件的產品。

1. 若要將其他條件行新增至陳述式，請返回步驟1並重複此程式，直到所有需要的條件完成為止。

   您可以隨時按一下「刪除」(![刪除圖示](assets/btn-del-red.png))圖示。
