---
title: Amazon sales channel — 標準價格規則動作
description: 使用標準價格規則動作，以增加或減少相對於Commerce目錄價格（或價格來源）的Amazon掛牌價格。
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# 標準價格規則動作

Amazon標準價格規則動作可讓您依照特定百分比或相對於 [!DNL Commerce] 型錄價格（或價格來源）。

標準價格規則動作的區段包括：

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 設定價格規則動作

1. 的 **[!UICONTROL Rule Type]**，選擇 `Standard price rule`.

   此選項會停用 _[!UICONTROL Select Rule Type]_區段。

1. 展開 _[!UICONTROL Price Adjustment]_區段（如有需要）。

1. 的 **[!UICONTROL Price Action]**，選擇一個選項以決定要如何變更 *[!UICONTROL Magento Price Source]* (定義於 [上市價格](./listing-price.md))值。

   - `Decrease By`  — 選擇您想要在列為Amazon之前減少值的時間。

   - `Increase By`  — 選擇您想要在列為Amazon之前增加值的時間。

1. 的 **[!UICONTROL Apply]**，選擇一個選項以決定要如何定義 *[!UICONTROL Magento Price Source]* 已在以下專案中定義： [上市價格](./listing-price.md) 要調整的值：

   - `Apply as percentage`  — 選擇您想要定義何時 *[!UICONTROL Magento Price Source]* 已在以下專案中定義： [上市價格](./listing-price.md) 以百分比調整的值

   - `Apply as fixed amount`  — 選擇您想要定義何時 *[!UICONTROL Magento Price Source]* 已在以下專案中定義： [上市價格](./listing-price.md) 以固定金額調整的值。

1. 的 **[!UICONTROL Adjustment Amount]** （必要），輸入價格調整的數值。

   - 時間 *[!UICONTROL Apply]* 設為 `Apply as percentage`，輸入百分比值(範例： enter `25` 25%的價格調整)。

   - 時間 *[!UICONTROL Apply]* 設為 `Apply as fixed amount`，輸入固定數量的數值(範例： enter `25` 25美元的固定價格調整)。

1. 完成後，按一下 **[!UICONTROL Save pricing rule]**.

![標準價格規則](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | 選取 `Standard price rule`. |
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇您想要定義何時 [!DNL Commerce] 在列為Amazon之前應減少的價格來源值。</li><li>**[!UICONTROL Increase By]**  — 選擇您想要定義何時 [!DNL Commerce] 在列為Amazon之前要增加的價格來源值。</li></ul> |
| [!UICONTROL Apply] | 選項：<ul><li>**[!UICONTROL Apply as percentage]**  — 選擇您想要定義何時 [!DNL Commerce] 以百分比調整的價格來源值。</li><li>**[!UICONTROL Apply as fixed amount]**  — 選擇您想要定義何時 [!DNL Commerce] 由固定金額調整的價格來源值。</li></ul> |
| [!UICONTROL Adjustment Amount] | 必填。<br><br>如果您選擇 `Apply as percentage` 的 *[!UICONTROL Apply]*，輸入百分比值(範例： enter `25` 25%的調整)。<br><br>如果您選擇 `Apply as fixed amount` 的 *[!UICONTROL Apply]*，輸入固定數量的數值(範例： enter `25` 25美元的固定調整)。 |
