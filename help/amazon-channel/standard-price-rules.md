---
title: 標準價格規則活動
description: 使用標準價格規則操作可以相對於Commerce目錄價格（或價格來源）增加或減少Amazon上市價格。
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 標準價格規則活動

標準價格規則活動允許您將Amazon的上市價格相對於 [!DNL Commerce] 目錄價格（或價格來源）。

標準價格規則活動的部分包括：

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 配置價格規則操作

1. 對於 **[!UICONTROL Rule Type]**&#x200B;選項 `Standard price rule`。

   此選項禁用 _[!UICONTROL Select Rule Type]_的子菜單。

1. 展開 _[!UICONTROL Price Adjustment]_的子菜單。

1. 對於 **[!UICONTROL Price Action]**，選擇一個選項以確定要如何更改 *[!UICONTROL Magento Price Source]* (定義於 [上市價格](./listing-price.md))值。

   - `Decrease By`  — 在列入Amazon之前，選擇希望值減少的時間。

   - `Increase By`  — 在列入Amazon之前，選擇希望何時增加值。

1. 對於 **[!UICONTROL Apply]**，選擇一個選項和一個選項，以確定要如何定義 *[!UICONTROL Magento Price Source]* 定義 [上市價格](./listing-price.md) 調整值：

   - `Apply as percentage`  — 選擇何時要定義 *[!UICONTROL Magento Price Source]* 定義 [上市價格](./listing-price.md) 按百分比調整的值

   - `Apply as fixed amount`  — 選擇何時要定義 *[!UICONTROL Magento Price Source]* 定義 [上市價格](./listing-price.md) 按固定金額調整的值。

1. 對於 **[!UICONTROL Adjustment Amount]** （必需），輸入價格調整的數值。

   - 當 *[!UICONTROL Apply]* 設定為 `Apply as percentage`，輸入百分比值(例如：輸入 `25` 價格調整25%)。

   - 當 *[!UICONTROL Apply]* 設定為 `Apply as fixed amount`，輸入固定金額的數值(例如：輸入 `25` 25美元的固定價格調整)。

1. 完成後，按一下 **[!UICONTROL Save pricing rule]**。

![標準價格規則](assets/ob-price-rule-action-standard-example.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Rule Type] | 選擇 `Standard price rule`。 |
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇何時要定義 [!DNL Commerce] 價格來源價值在上市前應減少至Amazon。</li><li>**[!UICONTROL Increase By]**  — 選擇何時要定義 [!DNL Commerce] 在上市前將增加價格來源價值。</li></ul> |
| [!UICONTROL Apply] | 選項：<ul><li>**[!UICONTROL Apply as percentage]**  — 選擇何時要定義 [!DNL Commerce] 價格來源值按百分比調整。</li><li>**[!UICONTROL Apply as fixed amount]**  — 選擇何時要定義 [!DNL Commerce] 價格來源值按固定金額調整。</li></ul> |
| [!UICONTROL Adjustment Amount] | 必需。<br><br>如果您選擇 `Apply as percentage` 為 *[!UICONTROL Apply]*，輸入百分比值(例如：輸入 `25` 調整25%)。<br><br>如果您選擇 `Apply as fixed amount` 為 *[!UICONTROL Apply]*，輸入固定金額的數值(例如：輸入 `25` 25美元的固定調整)。 |
