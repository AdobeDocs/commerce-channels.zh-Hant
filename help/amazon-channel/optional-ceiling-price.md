---
title: 「智慧型重新訂價規則：選擇性上限價格」
description: 使用選用的上限價格設定，可針對管理Amazon清單的智慧定價規則，保護您的最高產品價格。
feature: Sales Channels, Price Rules
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b2e608a633b760672044653a22be757ecffc9540
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 智慧型重新訂價規則：選擇性上限價格

智慧型重新訂價規則的區段包括：

- [選取規則型別](./intelligent-repricing-rules.md)
- [競爭者條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [底價](./floor-price.md)
- 選擇性最高價格

自動上限價格設定會自動根據智慧型訂價規則保護您的最高產品價格，讓您為智慧型訂價規則設定上限（最高價格）。

## 設定可選的上限價格

在&#x200B;_[!UICONTROL Optional Ceiling Price]_區段中定義您選擇性的最高價格設定。

1. 針對&#x200B;**[!UICONTROL Ceiling Price Source]**，選擇屬性。

   選取您的[!DNL Commerce] [產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)，指出您的相對上限限制。 例如，如果您不希望Amazon清單價格高於專案的MSRP，您可以選擇`Manufacturer's Suggested Retail Price`屬性。

1. 針對&#x200B;**[!UICONTROL Ceiling Price Action]**，選擇一個選項。

   - `Decrease By` — 選擇您何時想要向下調整定義的&#x200B;_[!UICONTROL Ceiling Price Source]_值，為規則建立較低的最高價格，然後再列為Amazon。

   - `Increase By` — 選擇您何時想要調整定義的&#x200B;_[!UICONTROL Ceiling Price Source]_值，為規則建立更高的最高價格，然後再列為Amazon。

   - `Match` — 選擇何時不希望清單價格波動超過定義的&#x200B;_[!UICONTROL Ceiling Price Source]_值。 設定為`Match`時，_[!UICONTROL Apply]_&#x200B;和&#x200B;_[!UICONTROL Ceiling Adjustment Amount]_欄位會停用。

1. 保留&#x200B;**[!UICONTROL Apply]**&#x200B;預設為`Apply as percentage`。

1. 針對&#x200B;**[!UICONTROL Ceiling Adjustment Price]**，輸入百分比的數值，以調整您的&#x200B;_[!UICONTROL Ceiling Price Source]_值。

在此範例中，最高價格設定為比料號的MSRP低2%。

![智慧型重新訂價規則 — 選擇性最高價格](assets/ob-intelligent-price-rule-ceiling.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|---------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Ceiling Price Source] | 選擇代表您相對上限的[!DNL Commerce] [產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)。 例如，如果您不想讓產品清單價格高於專案的MSRP，您可以選擇`Manufacturer's Suggested Retail Price`屬性。 |
| [!UICONTROL Ceiling Price Action] | 選擇訂價調整作業。 選項：<ul><li>**[!UICONTROL Decrease By]** — 選擇您何時想要向下調整定義的&#x200B;_[!UICONTROL Ceiling Price Source]_值，為規則建立較低的最高價格，然後再列為Amazon。</li><li>**[!UICONTROL Increase By]** — 選擇您何時想要調整定義的&#x200B;_[!UICONTROL Ceiling Price Source]_值，為規則建立更高的最高價格，然後再列為Amazon。</li><li>**[!UICONTROL Match]** — 選擇何時不希望清單價格波動超過定義的&#x200B;_[!UICONTROL Ceiling Price Source]_值。 設定為`Match`時，_[!UICONTROL Apply]_&#x200B;和&#x200B;_[!UICONTROL Ceiling Adjustment Amount]_欄位會停用。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** — 相對於&#x200B;_[!UICONTROL Ceiling Price Source]_值的百分比調整。 |
| [!UICONTROL Ceiling Price Adjustment] | 輸入百分比的數值，以調整您的&#x200B;_[!UICONTROL Ceiling Price Source]_值。 |
