---
title: 「智慧重新定價規則：最低價格'
description: 使用底價設定來決定智慧定價規則的最低價格，以管理您的Amazon清單。
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 智慧重新定價規則：底價

智慧重新定價規則的章節包括：

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

此 [底價](./floor-price.md) 設定會自動保護您最低的產品價格，不受智慧定價規則的影響。 使用這些設定為智慧定價規則設定下限（最低價格），確保您的產品不會以低於所需價格的價格列出。

價格下限屬性是根據網站範圍(若您 [!DNL Commerce] 商店使用網站定價範圍。 請參閱 [價格範圍](./price-scope.md).

只有在 **[!UICONTROL Rule Type]** 設為 `Intelligent repricing rule`.

## 配置底價

在 _[!UICONTROL Floor Price]_區段。

1. 針對 **[!UICONTROL Floor Price Source]**，選擇價格來源屬性。

   選擇 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target=&quot;_blank&quot;}，表示您的相對下限。 例如，若您不希望Amazon清單價格低於項目成本，您可以選擇 *成本* 屬性。

1. 針對 **[!UICONTROL Floor Price Action]**，選擇選項。

   - `Decrease By`  — 選擇要定義的時間 _[!UICONTROL Floor Price Source]_值需向下調整，為規則建立較低的底價，再上市至Amazon。

   - `Increase By`  — 選擇要定義的時間 _[!UICONTROL Floor Price Source]_價值需加以調整，為規則建立較高的底價，然後再上市至Amazon。

   - `Match`  — 選擇您不希望上市價格在定義 _[!UICONTROL Floor Price Source]_值。 設為時 `Match`,_[!UICONTROL Apply]_ 和 _[!UICONTROL Floor Adjustment Amount]_欄位已停用。

1. 保留 **[!UICONTROL Apply]** 預設為 `Apply as percentage`.

1. 針對 **[!UICONTROL Floor Adjustment Price]**，輸入百分比的數值以調整 _[!UICONTROL Floor Price Source]_值。

在此範例中，底價設為高於項目成本的3%。

![智慧重新定價規則範例 — 底價](assets/ob-intelligent-pricde-rule-floor-price.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Floor Price Source] | 選擇 [!DNL Commerce] 表示相對下限（最低價格）限制的屬性。 例如，若您不希望Amazon清單價格低於項目成本，您可以選擇 `Cost` 屬性。 |
| [!UICONTROL Floor Price Action] | 選擇定價調整活動。 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇要定義的時間 _[!UICONTROL Floor Price Source]_值需向下調整，為規則建立較低的底價，再上市至Amazon。</li><li>**[!UICONTROL Increase By]**  — 選擇要定義的時間 _[!UICONTROL Floor Price Source]_價值需加以調整，為規則建立較高的底價，然後再上市至Amazon。</li><li>**[!UICONTROL Match]**  — 選擇您不希望上市價格在定義 _[!UICONTROL Floor Price Source]_值。 選擇後，_[!UICONTROL Apply]_ 和 _[!UICONTROL Floor Adjustment Amount]_欄位已停用。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]**  — 相對於 _[!UICONTROL Floor Price Source]_值。 |
| [!UICONTROL Floor Adjustment Amount] | 輸入百分比的數值以調整 _[!UICONTROL Floor Price Source]_值。 |
