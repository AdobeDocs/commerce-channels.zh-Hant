---
title: Amazon sales channel — 價格規則條件
description: 使用價格規則條件來決定哪些產品符合上市價格規則的資格。
feature: Sales Channels, Price Rules
exl-id: 39b03a2e-15c6-4c56-b0e0-7c6823e95fa8
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 價格規則條件

條件會決定哪些產品符合價格規則的條件。 定義Amazon定價規則的條件，會遵循與在[!DNL Commerce]中定義[購物車價格規則](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html)的條件相同的邏輯和程式。

>[!IMPORTANT]
>
>如果您的價格規則套用至[!DNL Commerce]目錄中的所有產品，則請將此區段留空。

條件中任何粗體的區域都可以按一下，以檢視各種選項。

## 範例：建立價格規則條件

此程式可能簡單或詳細，視您的目錄設定而定。 您可以定義條件，以便當產品的`ALL`或`ANY`條件為`TRUE`或`FALSE`時，該產品符合套用的定價規則的資格。

條件是以您的[產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)為基礎。 若要將規則套用至所有產品，請將「條件」區段保留空白。

>[!NOTE]
>
>若要根據特定產品屬性定義條件，屬性的&#x200B;**用於促銷規則條件**&#x200B;必須在您屬性的[店面屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html)中設定為`Yes`。

![價格規則條件 — 第1行](assets/ob-price-rules-condition-1.png){width="600" zoomable="yes"}

此範例所定義的規則，可對`Books`類別中定義的所有產品套用25%折扣。

規則陳述式有兩個粗體連結，按一下連結時，會顯示條件陳述式該部分的選項。 如果您儲存條件而未變更粗體選項，則規則會套用至您的所有產品。

- 按一下&#x200B;**[!UICONTROL ALL]**&#x200B;並選擇`ALL`或`ANY`。
- 按一下&#x200B;**[!UICONTROL TRUE]**，然後選擇`TRUE`或`FALSE`。
- 若要將規則套用至所有產品，請保持條件不變。

您可以變更這些值的組合，以建立不同的條件。 在此範例中，會使用下列條件：

`If ALL of these conditions are TRUE:`

1. 若要顯示條件套用的可用屬性，請按一下條件行開頭的「新增」 （![「新增」圖示](assets/btn-add-grn.png)）圖示，並選取條件所依據的屬性。

   **[!UICONTROL Conditions Combination]** — 選擇在現有條件中建立另一組`All/Any`和`True/False`條件。

   ![價格規則條件組合](assets/ob-conditions-combinations.png){width="500"}

   **[!UICONTROL Product Attribute]** — 可用的產品屬性取決於屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/create/attribute-product-create.html)的[設定。 若要讓屬性顯示在清單中，您店面屬性中的&#x200B;*[!UICONTROL Use for Promo Rule Conditions]*&#x200B;必須設定為`Yes`。

   - 針對&#x200B;**[!UICONTROL Product Attribute]**，選擇您要定義為條件基底的屬性。 在此範例中，選取的條件是`Category`。

     ![價格規則條件 — 第2行，第2部分](assets/ob-price-rule-condition-2.png){width="500"}

     選取的條件會顯示在陳述式中，後面接著兩個粗體連結。 選項會依您選取的產品屬性而有所不同。

     設定屬性後，便無法編輯它。 若要變更屬性，您必須刪除該行並新增屬性。 您可以按一下行尾的刪除(![刪除圖示](assets/btn-del-red.png)圖示，刪除條件行。

   - 按一下&#x200B;**[!UICONTROL is]**，然後選擇描述產品符合條件的比較運運算元。

     在此範例中，比較運運算元為`is`。 可用的選項取決於上一步驟中選取的屬性，可能包括不同的比較選項。 選項可包含相符的值，但不包含或包含至少一個值，以及大於、等於和小於數字量。 在此範例中，選項為`is`和`is not`。

   - 按一下&#x200B;**[!UICONTROL ...]**&#x200B;並選擇條件所依據的屬性值。 選項視屬性的設定而定。

     系統可能會提示您選取選項或輸入條件的值。 在此範例中，欄位顯示為空白。 若要選取規則的類別，請按一下選擇器圖示（![選擇器圖示](assets/btn-chooser.png)）以顯示您的選取選項。 此規則適用於&#x200B;_書籍_，請選取&#x200B;**[!UICONTROL Books]**&#x200B;核取方塊。 系統會填入類別編號。 若要接受您的類別選擇，請按一下綠色勾號圖示（![勾號圖示](assets/btn-check-mark-green.png)）。

     ![價格規則條件 — 第2行，第3部分](assets/ob-price-rule-condition-3.png){width="500"}

     選取的專案會出現在陳述式中，以完成條件。

     ![價格規則條件 — 第2行，第4部分](assets/ob-price-rule-condition-4.png){width="500"}

     此範例條件已完成。 如上所述，此條件表示您[!DNL Commerce]目錄中擁有已定義之叢書類別(`4`)的任何產品均符合此定價規則的資格。 您可以新增更多條件行，進一步縮小合格產品的範圍。

1. 若要將另一個條件行加入陳述式，請回到步驟1並重複此程式，直到所有需要的條件都完成為止。

   您可以隨時刪除條件陳述式的一行，方法是按一下該行結尾的刪除（![刪除圖示](assets/btn-del-red.png)）圖示。
