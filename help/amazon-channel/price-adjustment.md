---
title: 價格調整
description: 配置價格調整以在您確定Amazon競爭者價格來源時定義價格計算。
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 價格調整

>[!NOTE]
>
>「價格調整」區段與「標準」和「智慧型」重新定價規則略有不同。 **[!UICONTROL Match Competitor Price]** 只有設為 _[!UICONTROL Price Action]_時&#x200B;**[!UICONTROL Rule Type]**才可在 `Intelligent repricing rule`下使用。

智慧重新定價規則的章節包括：

- [選擇規則類型](./intelligent-repricing-rules.md)
- [競爭者條件差異](./competitor-conditional-variances.md)
- 價格調整
- [最低價格](./floor-price.md)
- [可選最高價格](./optional-ceiling-price.md)

價格調整會在您確定競爭者價格來源時定義價格計算。

## 配置價格調整

在&#x200B;_[!UICONTROL Price Adjustment]_區段中定義定價調整。

1. 對於&#x200B;**[!UICONTROL Price Action]**，選擇一個選項：

   - `Decrease By`  — 選擇在將定義的價格來源值下調後，為規則建立較低的價格，然後再將其上市至Amazon。

   - `Increase By`  — 選擇何時要調整定義的價格來源值，為規則建立較高的價格，然後再上市至Amazon。

   - `Match Competitor Price`  — （僅限智慧型重新定價規則）根據您的競爭者意見和變異參數，選擇您要變更Amazon上市價 [格以](./lowest-competitor-pricing.md) 符合最低競爭者價格的時機。設為`Match Competitor Price`時，會移除&#x200B;_[!UICONTROL Apply]_和_[!UICONTROL Adjustment Amount]_&#x200B;欄位。

1. 對於&#x200B;**[!UICONTROL Apply]**，選擇一個選項：

   - `Apply as percentage`  — 選擇何時要以百 **[!UICONTROL Magento Price Source]** 分比調整 [上市](./listing-price.md) 價格中定義的。

   - `Apply as fixed amount`  — 選擇何時要將「上市價 **[!UICONTROL Magento Price Source]** 格」中定義的 [定](./listing-price.md) 義值調整為固定金額。

1. 對於&#x200B;**[!UICONTROL Adjustment Amount]**（必要），輸入價格調整的數值。

   - 當&#x200B;**[!UICONTROL Apply]**&#x200B;設為`Apply as percentage`時，輸入百分比值(範例：輸入`25`以獲得25%的調整)。

   - 當&#x200B;**[!UICONTROL Apply]**&#x200B;設為`Apply as fixed amount`時，輸入固定金額的數值(例如：輸入`25`以獲取$25的固定調整)。

![智慧重新定價規則 — 價格調整](assets/amazon-price-adjustment.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Price Action] | 選擇定價調整活動。 選項：<br>**[!UICONTROL Decrease By]**— 在[清單價格](./listing-price.md)中定義的&#x200B;_[!UICONTROL Magento Price Source]_需要向下調整時，選擇何時為規則建立較低的價格，再將其列入Amazon。<br>**[!UICONTROL Increase By]**— 選擇在上市前，_[!UICONTROL Magento Price Source]_ 何時 [調](./listing-price.md) 整上市價格中定義的規則，為規則建立更高的價格。<br>**[!UICONTROL Match Competitor Price]**— （僅限智慧型重新定價規則）根據您的競爭者意見和變異參數，選擇您要變更Amazon上市價 [格以](./lowest-competitor-pricing.md) 符合最低競爭者價格的時機。選擇&#x200B;_Apply_和&#x200B;_Adjustment Amount_欄位後，將刪除該欄位。 |
| [!UICONTROL Apply] | 選項：<br>**[!UICONTROL Apply as percentage]**— 選擇何時要在[清單價格](./listing-price.md)中定義的&#x200B;_[!UICONTROL Magento Price Source]_以百分比調整。<br>**[!UICONTROL Apply as fixed amount]**— 選擇何時要將「上市價_[!UICONTROL Magento Price Source]_ 格」中定義的 [定](./listing-price.md) 義值調整為固定金額。 |
| [!UICONTROL Adjustment Amount] | 必填。<br>如果您選 `Apply as percentage` 擇 **[!UICONTROL Apply]**&#x200B;用於，請輸入百分比值(例如：輸 `25` 入25%的調整)。<br>如果您選 `Apply as fixed amount` 擇 **[!UICONTROL Apply]**&#x200B;用於固定金額，請輸入數值(例如：輸 `25` 入$25固定調整)。 |
