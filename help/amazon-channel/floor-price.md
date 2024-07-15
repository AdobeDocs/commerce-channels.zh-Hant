---
title: 「智慧型重新訂價規則：底價」
description: 請使用底價設定來決定智慧型訂價規則的最低價格，以管理您的Amazon清單。
feature: Sales Channels, Price Rules
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 智慧型重新訂價規則：底價

智慧型重新訂價規則的區段包括：

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

[底價](./floor-price.md)設定會自動保護您最低的產品價格，不受智慧型定價規則的限制。 使用這些設定來設定智慧型定價規則的下限（最低價格），確保您的產品不會低於所要的價格。

若您的[!DNL Commerce]商店使用網站定價範圍，則底價屬性會以網站範圍為基礎。 檢視[價格範圍](./price-scope.md)。

只有當&#x200B;**[!UICONTROL Rule Type]**&#x200B;設定為`Intelligent repricing rule`時才使用底價。

## 設定底價

在&#x200B;_[!UICONTROL Floor Price]_區段中定義您的最低價格設定。

1. 針對&#x200B;**[!UICONTROL Floor Price Source]**，選擇價格來源屬性。

   選擇指示您相對樓層限制的[!DNL Commerce] [產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)。 例如，如果您不想讓Amazon清單價格低於專案的成本，您可以選擇&#x200B;*成本*&#x200B;屬性。

1. 針對&#x200B;**[!UICONTROL Floor Price Action]**，選擇一個選項。

   - `Decrease By` — 選擇您想要向下調整已定義的&#x200B;_[!UICONTROL Floor Price Source]_值，並為規則建立較低的底價，然後再列為Amazon。

   - `Increase By` — 選擇您何時想要調整已定義的&#x200B;_[!UICONTROL Floor Price Source]_值，以便建立更高的規則底價，然後再列為Amazon。

   - `Match` — 選擇何時不希望清單價格波動到定義的&#x200B;_[!UICONTROL Floor Price Source]_值以下。 設定為`Match`時，_[!UICONTROL Apply]_&#x200B;和&#x200B;_[!UICONTROL Floor Adjustment Amount]_欄位會停用。

1. 保留&#x200B;**[!UICONTROL Apply]**&#x200B;預設為`Apply as percentage`。

1. 針對&#x200B;**[!UICONTROL Floor Adjustment Price]**，輸入百分比的數值，以調整您的&#x200B;_[!UICONTROL Floor Price Source]_值。

在此範例中，底價設定為比料號成本高3%。

![智慧型重新訂價規則範例 — 底價](assets/ob-intelligent-pricde-rule-floor-price.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Floor Price Source] | 選擇表示您相對下限（最低價格）限制的[!DNL Commerce]屬性。 例如，如果您不希望您的Amazon清單價格低於專案的成本，您可以選擇`Cost`屬性。 |
| [!UICONTROL Floor Price Action] | 選擇訂價調整作業。 選項：<ul><li>**[!UICONTROL Decrease By]** — 選擇您想要向下調整已定義的&#x200B;_[!UICONTROL Floor Price Source]_值，並為規則建立較低的底價，然後再列為Amazon。</li><li>**[!UICONTROL Increase By]** — 選擇您何時想要調整已定義的&#x200B;_[!UICONTROL Floor Price Source]_值，以便建立更高的規則底價，然後再列為Amazon。</li><li>**[!UICONTROL Match]** — 選擇何時不希望清單價格波動到定義的&#x200B;_[!UICONTROL Floor Price Source]_值以下。 選擇後，_[!UICONTROL Apply]_&#x200B;和&#x200B;_[!UICONTROL Floor Adjustment Amount]_欄位會停用。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]** — 相對於&#x200B;_[!UICONTROL Floor Price Source]_值的百分比調整。 |
| [!UICONTROL Floor Adjustment Amount] | 輸入百分比的數值，以調整您的&#x200B;_[!UICONTROL Floor Price Source]_值。 |
