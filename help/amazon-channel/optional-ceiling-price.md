---
title: 「智慧重定價規則：可選上限價格`
description: 使用可選的上限價格設定，針對管理您的Amazon清單的智慧定價規則保護您的最高產品價格。
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# 智慧重定價規則：可選上限價格

智慧重新定價規則的部分包括：

- [選擇規則類型](./intelligent-repricing-rules.md)
- [競爭對手條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [底價](./floor-price.md)
- 可選上限價格

自動上限價格設定可自動保護您的最高產品價格不受智慧定價規則的影響，使您能夠為智慧定價規則設定上限（最高價格）。

## 配置可選上限價格

在 _[!UICONTROL Optional Ceiling Price]_的子菜單。

1. 對於 **[!UICONTROL Ceiling Price Source]**&#x200B;的子菜單。

   選擇 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 表示你的相對上限。 例如，如果您不希望您的Amazon清單價格高於物料的MSRP，則您將選擇 `Manufacturer's Suggested Retail Price` 屬性。

1. 對於 **[!UICONTROL Ceiling Price Action]**，也請參見Wiki頁。

   - `Decrease By`  — 選擇何時要定義 _[!UICONTROL Ceiling Price Source]_在上市前，將向下調整，為規則創造較低的上限價格。

   - `Increase By`  — 選擇何時要定義 _[!UICONTROL Ceiling Price Source]_價值要調整，為規則創造更高的上限價格，然後上市至Amazon。

   - `Match`  — 選擇不希望上市價格在定義價格之上波動時 _[!UICONTROL Ceiling Price Source]_值。 設定為時 `Match`，也請參見Wiki頁。_[!UICONTROL Apply]_ 和 _[!UICONTROL Ceiling Adjustment Amount]_欄位被禁用。

1. 離開 **[!UICONTROL Apply]** 預設為 `Apply as percentage`。

1. 對於 **[!UICONTROL Ceiling Adjustment Price]**，輸入百分比的數值以調整 _[!UICONTROL Ceiling Price Source]_值。

在本例中，最高價格設定為低於項目MSRP的2%。

![智慧重定價規則 — 可選上限價格](assets/ob-intelligent-price-rule-ceiling.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Ceiling Price Source] | 選擇 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"} 表示你的相對上限。 例如，如果您不希望產品清單價格高於物料的MSRP，則您將選擇 `Manufacturer's Suggested Retail Price` 屬性。 |
| [!UICONTROL Ceiling Price Action] | 選擇定價調整活動。 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇何時要定義 _[!UICONTROL Ceiling Price Source]_在上市前，將向下調整，為規則創造較低的上限價格。</li><li>**[!UICONTROL Increase By]**  — 選擇何時要定義 _[!UICONTROL Ceiling Price Source]_價值要調整，為規則創造更高的上限價格，然後上市至Amazon。</li><li>**[!UICONTROL Match]**  — 選擇不希望上市價格在定義價格之上波動時 _[!UICONTROL Ceiling Price Source]_值。 設定為時 `Match`，也請參見Wiki頁。_[!UICONTROL Apply]_ 和 _[!UICONTROL Ceiling Adjustment Amount]_欄位被禁用。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]**  — 相對於 _[!UICONTROL Ceiling Price Source]_值。 |
| [!UICONTROL Ceiling Price Adjustment] | 輸入百分比的數值以調整 _[!UICONTROL Ceiling Price Source]_值。 |
