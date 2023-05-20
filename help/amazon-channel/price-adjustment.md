---
title: 價格調整
description: 配置價格調整，以在您確定Amazon競爭對手的價格來源時定義價格計算。
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 價格調整

>[!NOTE]
>
>「價格調整」部分與「標準」和「智慧」重新定價規則略有不同。 **[!UICONTROL Match Competitor Price]** 僅在 _[!UICONTROL Price Action]_何時&#x200B;**[!UICONTROL Rule Type]**設定為 `Intelligent repricing rule`。

智慧重新定價規則的部分包括：

- [選擇規則類型](./intelligent-repricing-rules.md)
- [競爭對手條件差異](./competitor-conditional-variances.md)
- 價格調整
- [底價](./floor-price.md)
- [可選上限價格](./optional-ceiling-price.md)

價格調整在您確定競爭對手的價格來源時定義價格計算。

## 配置價格調整

在 _[!UICONTROL Price Adjustment]_的子菜單。

1. 對於 **[!UICONTROL Price Action]**，選擇選項：

   - `Decrease By`  — 選擇在將定義的價格來源值向下調整時，為規則建立較低的價格，然後將其列入Amazon。

   - `Increase By`  — 選擇何時調整定義的價格來源值，為規則建立更高的價格，然後將其列入Amazon。

   - `Match Competitor Price`  — （僅限智慧重定價規則）選擇何時更改Amazon上市價格以匹配 [最差競爭對手](./lowest-competitor-pricing.md) 價格，根據競爭對手的反饋和方差參數。 設定為時 `Match Competitor Price`，也請參見Wiki頁。 _[!UICONTROL Apply]_和_[!UICONTROL Adjustment Amount]_ 欄位。

1. 對於 **[!UICONTROL Apply]**，選擇選項：

   - `Apply as percentage`  — 選擇何時要定義 **[!UICONTROL Magento Price Source]** 定義 [上市價格](./listing-price.md) 按百分比調整。

   - `Apply as fixed amount`  — 選擇何時要定義 **[!UICONTROL Magento Price Source]** 定義 [上市價格](./listing-price.md) 按固定金額調整。

1. 對於 **[!UICONTROL Adjustment Amount]** （必需），輸入價格調整的數值。

   - 當 **[!UICONTROL Apply]** 設定為 `Apply as percentage`，輸入百分比值(例如：輸入 `25` 調整25%)。

   - 當 **[!UICONTROL Apply]** 設定為 `Apply as fixed amount`，輸入固定金額的數值(例如：輸入 `25` 25美元的固定調整)。

![智慧重定價規則 — 價格調整](assets/amazon-price-adjustment.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Price Action] | 選擇定價調整活動。 選項：<br>**[!UICONTROL Decrease By]**— 選擇何時要定義 _[!UICONTROL Magento Price Source]_定義 [上市價格](./listing-price.md) 在上市前，先向下調整，為規則創造更低的價格。<br>**[!UICONTROL Increase By]**— 選擇何時要定義_[!UICONTROL Magento Price Source]_ 定義 [上市價格](./listing-price.md) 在上市前，為規則設定更高的價格。<br>**[!UICONTROL Match Competitor Price]**— （僅限智慧重定價規則）選擇何時更改Amazon上市價格以匹配 [最差競爭對手](./lowest-competitor-pricing.md) 價格，根據競爭對手的反饋和方差參數。 選擇後， _應用_ 和 _調整金額_ 欄位。 |
| [!UICONTROL Apply] | 選項：<br>**[!UICONTROL Apply as percentage]**— 選擇何時要定義 _[!UICONTROL Magento Price Source]_定義 [上市價格](./listing-price.md) 按百分比調整。<br>**[!UICONTROL Apply as fixed amount]**— 選擇何時要定義_[!UICONTROL Magento Price Source]_ 定義 [上市價格](./listing-price.md) 按固定金額調整。 |
| [!UICONTROL Adjustment Amount] | 必需。<br>如果您選擇 `Apply as percentage` 為 **[!UICONTROL Apply]**，輸入百分比值(例如：輸入 `25` 調整25%)。<br>如果您選擇 `Apply as fixed amount` 為 **[!UICONTROL Apply]**，輸入固定金額的數值(例如：輸入 `25` 25美元的固定調整)。 |
