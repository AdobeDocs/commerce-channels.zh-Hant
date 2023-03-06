---
title: 標準價格規則動作
description: 使用標準價格規則動作，以相對於商務目錄價格（或價格來源）增加或減少Amazon上市價格。
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 標準價格規則動作

標準價格規則動作可讓您以相對於以下項目的特定百分比或固定美元金額，來增加或減少Amazon上市價格： [!DNL Commerce] 目錄價格（或價格來源）。

標準價格規則操作的部分包括：

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 配置價格規則操作

1. 針對 **[!UICONTROL Rule Type]**，選擇 `Standard price rule`.

   此選項會停用 _[!UICONTROL Select Rule Type]_區段。

1. 展開 _[!UICONTROL Price Adjustment]_區段（如果需要）。

1. 針對 **[!UICONTROL Price Action]**，選擇選項以決定您要如何變更 *[!UICONTROL Magento Price Source]* (定義於 [上市價](./listing-price.md))值。

   - `Decrease By`  — 在列入Amazon之前，選擇要降低值的時間。

   - `Increase By`  — 在列入Amazon之前，選擇要增加值的時間。

1. 針對 **[!UICONTROL Apply]**，選擇選項和選項，以決定您要如何定義 *[!UICONTROL Magento Price Source]* 定義於 [上市價](./listing-price.md) 值：

   - `Apply as percentage`  — 選擇要定義的時間 *[!UICONTROL Magento Price Source]* 定義於 [上市價](./listing-price.md) 以百分比調整的值

   - `Apply as fixed amount`  — 選擇要定義的時間 *[!UICONTROL Magento Price Source]* 定義於 [上市價](./listing-price.md) 值以固定金額調整。

1. 針對 **[!UICONTROL Adjustment Amount]** （必要），輸入價格調整的數值。

   - 當 *[!UICONTROL Apply]* 設為 `Apply as percentage`，請輸入百分比值(範例：輸入 `25` 25%的價格調整)。

   - 當 *[!UICONTROL Apply]* 設為 `Apply as fixed amount`，輸入固定金額的數值(例如：輸入 `25` 25美元固定價格調整)。

1. 完成後，按一下 **[!UICONTROL Save pricing rule]**.

![標準價格規則](assets/ob-price-rule-action-standard-example.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Rule Type] | 選擇 `Standard price rule`. |
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]**  — 選擇要定義的時間 [!DNL Commerce] 價格來源值將在上市至Amazon前降低。</li><li>**[!UICONTROL Increase By]**  — 選擇要定義的時間 [!DNL Commerce] 價格來源值在上市至Amazon前須增加。</li></ul> |
| [!UICONTROL Apply] | 選項：<ul><li>**[!UICONTROL Apply as percentage]**  — 選擇要定義的時間 [!DNL Commerce] 價格來源值（以百分比調整）。</li><li>**[!UICONTROL Apply as fixed amount]**  — 選擇要定義的時間 [!DNL Commerce] 價格來源值（以固定金額調整）。</li></ul> |
| [!UICONTROL Adjustment Amount] | 必填。<br><br>如果您選擇 `Apply as percentage` for *[!UICONTROL Apply]*，請輸入百分比值(範例：輸入 `25` 25%的調整)。<br><br>如果您選擇 `Apply as fixed amount` for *[!UICONTROL Apply]*，輸入固定金額的數值(例如：輸入 `25` 25美元固定調整)。 |
