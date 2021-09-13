---
title: 「智慧重新定價規則：可選最高價格'
description: 使用可選的最高價格設定，保護您的最高產品價格不受管理Amazon清單的智慧定價規則影響。
exl-id: edc40e6b-e71f-41a3-8d5f-8bb73ada42a3
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# 智慧重新定價規則：可選上限價格

智慧重新定價規則的章節包括：

- [選擇規則類型](./intelligent-repricing-rules.md)
- [競爭者條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [最低價格](./floor-price.md)
- 可選最高價格

自動的最高價格設定可自動保護您的最高產品價格不受智慧定價規則的影響，使您能夠為智慧定價規則設定最高價格（最高價格）。

## 配置可選最高價格

在&#x200B;_[!UICONTROL Optional Ceiling Price]_區段中定義選用的最高價格設定。

1. 對於&#x200B;**[!UICONTROL Ceiling Price Source]**，選擇一個屬性。

   選擇[!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}，以指示您的相對上限限制。 例如，若您不希望Amazon的清單價格高於項目的MSRP，則可選擇`Manufacturer's Suggested Retail Price`屬性。

1. 對於&#x200B;**[!UICONTROL Ceiling Price Action]**，選擇一個選項。

   - `Decrease By`  — 選擇您要在將定 _[!UICONTROL Ceiling Price Source]_義的值向下調整的時間，為規則建立較低的上限價格，然後再將其列入Amazon。

   - `Increase By`  — 選擇您要何時調整 _[!UICONTROL Ceiling Price Source]_已定義的值，為規則建立較高的上限價格，然後再上市至Amazon。

   - `Match`  — 選擇不希望上市價格高於定義值的時 _[!UICONTROL Ceiling Price Source]_間。設為`Match`時，會停用_[!UICONTROL Apply]_&#x200B;和&#x200B;_[!UICONTROL Ceiling Adjustment Amount]_欄位。

1. 將&#x200B;**[!UICONTROL Apply]**&#x200B;預設值保留為`Apply as percentage`。

1. 對於&#x200B;**[!UICONTROL Ceiling Adjustment Price]**，輸入百分比的數值以調整&#x200B;_[!UICONTROL Ceiling Price Source]_值。

在此範例中，最高價格設為低於項目MSRP的2%。

![智慧重新定價規則 — 可選最高價格](assets/ob-intelligent-price-rule-ceiling.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Ceiling Price Source] | 選擇[!DNL Commerce] [product屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){:target=&quot;_blank&quot;}，以指示您的相對上限。 例如，若您不希望產品清單價格高於項目的MSRP，則會選擇`Manufacturer's Suggested Retail Price`屬性。 |
| [!UICONTROL Ceiling Price Action] | 選擇定價調整活動。 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇您要在將定 _[!UICONTROL Ceiling Price Source]_義的值向下調整的時間，為規則建立較低的上限價格，然後再將其列入Amazon。</li><li>**[!UICONTROL Increase By]**  — 選擇您要何時調整 _[!UICONTROL Ceiling Price Source]_已定義的值，為規則建立較高的上限價格，然後再上市至Amazon。</li><li>**[!UICONTROL Match]**  — 選擇不希望上市價格高於定義值的時 _[!UICONTROL Ceiling Price Source]_間。設為`Match`時，會停用_[!UICONTROL Apply]_&#x200B;和&#x200B;_[!UICONTROL Ceiling Adjustment Amount]_欄位。</li></ul> |
| [!UICONTROL Apply] | **[!UICONTROL Apply as percentage]**  — 相對於值的百分比調 _[!UICONTROL Ceiling Price Source]_整。 |
| [!UICONTROL Ceiling Price Adjustment] | 輸入百分比的數值以調整&#x200B;_[!UICONTROL Ceiling Price Source]_值。 |
