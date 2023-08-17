---
title: Amazon Sales Channel - [!UICONTROL Price Adjustment]
description: 設定價格調整，以便在您識別Amazon競爭者價格來源時定義價格計算。
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>「價格調整」區段的「標準」與「智慧」重新訂價規則稍有不同。 **[!UICONTROL Match Competitor Price]** 僅適用於 _[!UICONTROL Price Action]_當&#x200B;**[!UICONTROL Rule Type]**設為 `Intelligent repricing rule`.

智慧型重新訂價規則的區段包括：

- [選取規則型別](./intelligent-repricing-rules.md)
- [競爭者條件差異](./competitor-conditional-variances.md)
- 價格調整
- [底價](./floor-price.md)
- [選擇性最高價格](./optional-ceiling-price.md)

當您識別競爭對手的價格來源時，價格調整會定義價格計算。

## 設定價格調整

定義您的訂價調整，位於 _[!UICONTROL Price Adjustment]_區段。

1. 的 **[!UICONTROL Price Action]**，選擇一個選項：

   - `Decrease By`  — 選擇您何時希望向下調整已定義的價格來源值，以便針對規則建立較低的價格，然後再列示至Amazon。

   - `Increase By`  — 選擇您想要調整已定義價格來源值的時間，以便針對規則建立較高的價格，然後再列至Amazon。

   - `Match Competitor Price` - （僅限智慧型重新訂價規則）選擇何時要變更Amazon上市價格以符合 [最低競爭者](./lowest-competitor-pricing.md) 價格，根據競爭者的意見反應和差異引數而定。 當設定為 `Match Competitor Price`，則 _[!UICONTROL Apply]_和_[!UICONTROL Adjustment Amount]_ 欄位會遭到移除。

1. 的 **[!UICONTROL Apply]**，選擇一個選項：

   - `Apply as percentage`  — 選擇您想要定義何時 **[!UICONTROL Magento Price Source]** 已在以下專案中定義： [上市價格](./listing-price.md) 依百分比調整。

   - `Apply as fixed amount`  — 選擇您想要定義何時 **[!UICONTROL Magento Price Source]** 已在以下專案中定義： [上市價格](./listing-price.md) 依固定金額調整。

1. 的 **[!UICONTROL Adjustment Amount]** （必要），輸入價格調整的數值。

   - 時間 **[!UICONTROL Apply]** 設為 `Apply as percentage`，輸入百分比值(範例： enter `25` 25%的調整)。

   - 時間 **[!UICONTROL Apply]** 設為 `Apply as fixed amount`，輸入固定數量的數值(範例： enter `25` 25美元的固定調整)。

![智慧型重新訂價規則 — 價格調整](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | 選擇訂價調整作業。 選項：<br>**[!UICONTROL Decrease By]**— 選擇您想要定義何時 _[!UICONTROL Magento Price Source]_已在以下專案中定義： [上市價格](./listing-price.md) 將規則向下調整，在列為Amazon之前，請降低規則的價格。<br>**[!UICONTROL Increase By]**— 選擇您想要定義何時_[!UICONTROL Magento Price Source]_ 已在以下專案中定義： [上市價格](./listing-price.md) 即將調整，在列為Amazon之前，針對規則建立較高的價格。<br>**[!UICONTROL Match Competitor Price]**- （僅限智慧型重新訂價規則）選擇何時要變更Amazon上市價格以符合 [最低競爭者](./lowest-competitor-pricing.md) 價格，根據競爭者的意見反應和差異引數而定。 選擇後， _套用_ 和 _調整金額_ 欄位會遭到移除。 |
| [!UICONTROL Apply] | 選項：<br>**[!UICONTROL Apply as percentage]**— 選擇您想要定義何時 _[!UICONTROL Magento Price Source]_已在以下專案中定義： [上市價格](./listing-price.md) 依百分比調整。<br>**[!UICONTROL Apply as fixed amount]**— 選擇您想要定義何時_[!UICONTROL Magento Price Source]_ 已在以下專案中定義： [上市價格](./listing-price.md) 依固定金額調整。 |
| [!UICONTROL Adjustment Amount] | 必填。<br>如果您選擇 `Apply as percentage` 的 **[!UICONTROL Apply]**，輸入百分比值(範例： enter `25` 25%的調整)。<br>如果您選擇 `Apply as fixed amount` 的 **[!UICONTROL Apply]**，輸入固定數量的數值(範例： enter `25` 25美元的固定調整)。 |
