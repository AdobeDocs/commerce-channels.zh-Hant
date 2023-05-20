---
title: 「智慧重定價規則：底價`
description: 使用底價設定來確定智慧定價規則的最低價格，以管理您的Amazon清單。
exl-id: e00cac95-eef8-4d4d-b578-287a91f54bdf
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 智慧重定價規則：底價

智慧重新定價規則的部分包括：

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md)
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [!UICONTROL Floor Price]
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

的 [底價](./floor-price.md) 設定將自動保護您的最低產品價格，使其不受智慧定價規則的影響。 使用這些設定為智慧定價規則設定底價（最低價格），確保產品不低於所需價格。

如果您 [!DNL Commerce] 商店使用網站定價範圍。 請參閱 [價格範圍](./price-scope.md)。

最低價格僅在 **[!UICONTROL Rule Type]** 設定為 `Intelligent repricing rule`。

## 配置底價

定義中的最低價格設定 _[!UICONTROL Floor Price]_的子菜單。

1. 對於 **[!UICONTROL Floor Price Source]**，選擇價格來源屬性。

   選擇 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 表示你的相對地限。 例如，如果您不希望您的Amazon清單價格低於物料成本，則您將選擇 *成本* 屬性。

1. 對於 **[!UICONTROL Floor Price Action]**，也請參見Wiki頁。

   - `Decrease By`  — 選擇何時要定義 _[!UICONTROL Floor Price Source]_價值將向下調整，為規則創造較低的底價，然後上市至Amazon。

   - `Increase By`  — 選擇何時要定義 _[!UICONTROL Floor Price Source]_價值要向上調整，為規則創造較高的底價，然後再上市至Amazon。

   - `Match`  — 選擇不希望上市價格在定義價格之下波動 _[!UICONTROL Floor Price Source]_值。 設定為時 `Match`，也請參見Wiki頁。_[!UICONTROL Apply]_ 和 _[!UICONTROL Floor Adjustment Amount]_欄位被禁用。

1. 離開 **[!UICONTROL Apply]** 預設為 `Apply as percentage`。

1. 對於 **[!UICONTROL Floor Adjustment Price]**，輸入百分比的數值以調整 _[!UICONTROL Floor Price Source]_值。

在本例中，底價設定為比項目成本高3%。

![智慧重定價規則示例 — 底價](assets/ob-intelligent-pricde-rule-floor-price.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Floor Price Source] | 選擇 [!DNL Commerce] 表示相對下限（最低價格）限制的屬性。 例如，如果您不希望您的Amazon清單價格低於物料成本，則您將選擇 `Cost` 屬性。 |
| [!UICONTROL Floor Price Action] | 選擇定價調整活動。 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇何時要定義 _[!UICONTROL Floor Price Source]_價值將向下調整，為規則創造較低的底價，然後上市至Amazon。</li><li>**[!UICONTROL Increase By]**  — 選擇何時要定義 _[!UICONTROL Floor Price Source]_價值要向上調整，為規則創造較高的底價，然後再上市至Amazon。</li><li>**[!UICONTROL Match]**  — 選擇不希望上市價格在定義價格之下波動 _[!UICONTROL Floor Price Source]_值。 選擇後，_[!UICONTROL Apply]_ 和 _[!UICONTROL Floor Adjustment Amount]_欄位被禁用。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]**  — 相對於 _[!UICONTROL Floor Price Source]_值。 |
| [!UICONTROL Floor Adjustment Amount] | 輸入百分比的數值以調整 _[!UICONTROL Floor Price Source]_值。 |
