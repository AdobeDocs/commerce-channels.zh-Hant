---
title: Amazon銷售管道 — [!UICONTROL Price Adjustment]
description: 設定價格調整，以便在您識別Amazon競爭者價格來源時定義價格計算。
feature: Sales Channels, Price Rules
exl-id: 60569b37-2a6d-40ef-bcec-2c3a132a07e0
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# [!UICONTROL Price Adjustment]

>[!NOTE]
>
>「價格調整」區段的「標準」與「智慧」重新訂價規則稍有不同。 當&#x200B;**[!UICONTROL Rule Type]**&#x200B;設定為`Intelligent repricing rule`時，**[!UICONTROL Match Competitor Price]**&#x200B;僅可在&#x200B;_[!UICONTROL Price Action]_下使用。

智慧型重新訂價規則的區段包括：

- [選取規則型別](./intelligent-repricing-rules.md)
- [競爭者條件差異](./competitor-conditional-variances.md)
- 價格調整
- [底價](./floor-price.md)
- [選擇性最高價格](./optional-ceiling-price.md)

當您識別競爭對手的價格來源時，價格調整會定義價格計算。

## 設定價格調整

在&#x200B;_[!UICONTROL Price Adjustment]_區段中定義您的價格調整。

1. 針對&#x200B;**[!UICONTROL Price Action]**，選擇一個選項：

   - `Decrease By` — 選擇您何時希望向下調整定義的價格來源值，以便為規則建立較低的價格，然後再列示到Amazon。

   - `Increase By` — 選擇您何時想要調整定義的價格來源值，以便為規則建立較高的價格，然後再列為Amazon。

   - `Match Competitor Price` - （僅限智慧型重新訂價規則）根據競爭者意見反應和差異引數，選擇何時要變更Amazon清單價格以符合[最低競爭者](./lowest-competitor-pricing.md)價格。 設定為`Match Competitor Price`時，會移除&#x200B;_[!UICONTROL Apply]_和_[!UICONTROL Adjustment Amount]_&#x200B;欄位。

1. 針對&#x200B;**[!UICONTROL Apply]**，選擇一個選項：

   - `Apply as percentage` — 選擇何時要在您的[清單價格](./listing-price.md)中定義定義的&#x200B;**[!UICONTROL Magento Price Source]**&#x200B;以百分比調整。

   - `Apply as fixed amount` — 當您想要以固定金額調整在[清單價格](./listing-price.md)中定義的&#x200B;**[!UICONTROL Magento Price Source]**&#x200B;時，請選擇此選項。

1. 針對&#x200B;**[!UICONTROL Adjustment Amount]** （必要），輸入價格調整的數值。

   - 當&#x200B;**[!UICONTROL Apply]**&#x200B;設定為`Apply as percentage`時，請輸入百分比值（例如：輸入`25`以調整25%的百分比）。

   - 當&#x200B;**[!UICONTROL Apply]**&#x200B;設定為`Apply as fixed amount`時，請輸入固定金額的數值（例如：輸入`25`作為$25的固定調整）。

![智慧型重新訂價規則 — 價格調整](assets/amazon-price-adjustment.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Price Action] | 選擇訂價調整作業。 選項：<br>**[!UICONTROL Decrease By]**— 選擇何時要在列出至Amazon之前，將您在[清單價格](./listing-price.md)中定義的&#x200B;_[!UICONTROL Magento Price Source]_向下調整，以建立較低的規則價格。<br>**[!UICONTROL Increase By]**— 當您想要調整在[清單價格](./listing-price.md)中定義的_[!UICONTROL Magento Price Source]_&#x200B;時，請選擇時機，以便為規則建立更高的價格，然後再列在Amazon中。<br>**[!UICONTROL Match Competitor Price]**- （僅限智慧型重新訂價規則）根據競爭者意見反應和差異引數，選擇何時要變更Amazon清單價格以符合[最低競爭者](./lowest-competitor-pricing.md)價格。 選取時，會移除&#x200B;_套用_與&#x200B;_調整金額_欄位。 |
| [!UICONTROL Apply] | 選項：<br>**[!UICONTROL Apply as percentage]**— 選擇何時要在您的[清單價格](./listing-price.md)中定義定義的&#x200B;_[!UICONTROL Magento Price Source]_以百分比調整。<br>**[!UICONTROL Apply as fixed amount]**— 當您想要以固定金額調整在[清單價格](./listing-price.md)中定義的_[!UICONTROL Magento Price Source]_&#x200B;時，請選擇此選項。 |
| [!UICONTROL Adjustment Amount] | 必填。<br>如果您選擇`Apply as percentage`作為&#x200B;**[!UICONTROL Apply]**，請輸入百分比值（例如：輸入`25`作為25%的百分比調整）。<br>如果您選擇`Apply as fixed amount`作為&#x200B;**[!UICONTROL Apply]**，請輸入固定金額的數值（例如：輸入`25`作為$25固定調整）。 |
