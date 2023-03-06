---
title: 「智慧重新定價規則：可選最高價格'
description: 使用可選的最高價格設定，保護您的最高產品價格不受管理Amazon清單的智慧定價規則影響。
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# 智慧重新定價規則：可選最高價格

智慧重新定價規則的章節包括：

- [選擇規則類型](./intelligent-repricing-rules.md)
- [競爭者條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [最低價格](./floor-price.md)
- 可選最高價格

自動的最高價格設定可自動保護您的最高產品價格不受智慧定價規則的影響，使您能夠為智慧定價規則設定最高價格（最高價格）。

## 配置可選最高價格

在 _[!UICONTROL Optional Ceiling Price]_區段。

1. 針對 **[!UICONTROL Ceiling Price Source]**，選擇屬性。

   選取 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 表示你的相對上限。 例如，若您不希望Amazon的清單價格高於項目的MSRP，您可以選擇 `Manufacturer's Suggested Retail Price` 屬性。

1. 針對 **[!UICONTROL Ceiling Price Action]**，選擇選項。

   - `Decrease By`  — 選擇要定義的時間 _[!UICONTROL Ceiling Price Source]_值需向下調整，為規則建立較低的上限價格，再上市至Amazon。

   - `Increase By`  — 選擇要定義的時間 _[!UICONTROL Ceiling Price Source]_價值需加以調整，為規則建立較高的上限價格，然後才上市至Amazon。

   - `Match`  — 選擇您不希望上市價格高於已定義 _[!UICONTROL Ceiling Price Source]_值。 設為時 `Match`,_[!UICONTROL Apply]_ 和 _[!UICONTROL Ceiling Adjustment Amount]_欄位已停用。

1. 保留 **[!UICONTROL Apply]** 預設為 `Apply as percentage`.

1. 針對 **[!UICONTROL Ceiling Adjustment Price]**，輸入百分比的數值以調整 _[!UICONTROL Ceiling Price Source]_值。

在此範例中，最高價格設為低於項目MSRP的2%。

![智慧重新定價規則 — 可選最高價格](assets/ob-intelligent-price-rule-ceiling.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Ceiling Price Source] | 選擇 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 表示你的相對上限。 例如，若您不希望產品清單價格高於項目的MSRP，您可以選擇 `Manufacturer's Suggested Retail Price` 屬性。 |
| [!UICONTROL Ceiling Price Action] | 選擇定價調整活動。 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇要定義的時間 _[!UICONTROL Ceiling Price Source]_值需向下調整，為規則建立較低的上限價格，再上市至Amazon。</li><li>**[!UICONTROL Increase By]**  — 選擇要定義的時間 _[!UICONTROL Ceiling Price Source]_價值需加以調整，為規則建立較高的上限價格，然後才上市至Amazon。</li><li>**[!UICONTROL Match]**  — 選擇您不希望上市價格高於已定義 _[!UICONTROL Ceiling Price Source]_值。 設為時 `Match`,_[!UICONTROL Apply]_ 和 _[!UICONTROL Ceiling Adjustment Amount]_欄位已停用。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]**  — 相對於 _[!UICONTROL Ceiling Price Source]_值。 |
| [!UICONTROL Ceiling Price Adjustment] | 輸入百分比的數值以調整 _[!UICONTROL Ceiling Price Source]_值。 |
