---
title: Amazon sales channel — 標準價格規則動作
description: 使用標準價格規則動作，以增加或減少相對於Amazon目錄價格（或價格來源）的Commerce掛牌價格。
feature: Sales Channels, Price Rules
exl-id: 91df6ef3-852b-478b-8b01-51dd437dd4f9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 標準價格規則動作

標準價格規則動作可讓您以特定百分比或相對於[!DNL Commerce]目錄價格（或價格來源）的固定金額來增減Amazon掛牌價格。

標準價格規則動作的區段包括：

- [!UICONTROL Select Rule Type]
- [!UICONTROL Price Adjustment]

## 設定價格規則動作

1. 針對&#x200B;**[!UICONTROL Rule Type]**，請選擇`Standard price rule`。

   此選項會停用&#x200B;_[!UICONTROL Select Rule Type]_區段中的其他欄位。

1. 視需要展開&#x200B;_[!UICONTROL Price Adjustment]_區段。

1. 針對&#x200B;**[!UICONTROL Price Action]**，選擇選項以決定您要如何變更&#x200B;*[!UICONTROL Magento Price Source]* （定義於您的[清單價格](./listing-price.md)）值。

   - `Decrease By` — 選擇您想要在列為Amazon之前減少值的時間。

   - `Increase By` — 選擇您想要在列為Amazon之前增加值的時間。

1. 針對&#x200B;**[!UICONTROL Apply]**，選擇選項以決定您要如何調整[清單價格](./listing-price.md)值中定義的&#x200B;*[!UICONTROL Magento Price Source]*：

   - `Apply as percentage` — 選擇您何時要在您的[清單價格](./listing-price.md)值中定義定義的&#x200B;*[!UICONTROL Magento Price Source]*，並以百分比調整

   - `Apply as fixed amount` — 當您想要在[清單價格](./listing-price.md)值中定義定義的&#x200B;*[!UICONTROL Magento Price Source]*&#x200B;以固定金額調整時，請選擇此選項。

1. 針對&#x200B;**[!UICONTROL Adjustment Amount]** （必要），輸入價格調整的數值。

   - 當&#x200B;*[!UICONTROL Apply]*&#x200B;設定為`Apply as percentage`時，請輸入百分比值（範例：輸入`25`以進行25%的價格調整）。

   - 當&#x200B;*[!UICONTROL Apply]*&#x200B;設定為`Apply as fixed amount`時，請輸入固定金額的數值（例如：輸入`25`進行$25的固定價格調整）。

1. 完成時，按一下&#x200B;**[!UICONTROL Save pricing rule]**。

![標準價格規則](assets/ob-price-rule-action-standard-example.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|--------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Rule Type] | 選取`Standard price rule`。 |
| [!UICONTROL Price Action] | 選項：<ul><li>**[!UICONTROL Decrease By]** — 選擇您要在將定義的[!DNL Commerce]價格來源值列為Amazon之前減少的時間。</li><li>**[!UICONTROL Increase By]** — 選擇您何時希望定義的[!DNL Commerce]價格來源值在列為Amazon之前增加。</li></ul> |
| [!UICONTROL Apply] | 選項：<ul><li>**[!UICONTROL Apply as percentage]** — 當您想要以百分比調整定義的[!DNL Commerce]價格來源值時，請選擇此選項。</li><li>**[!UICONTROL Apply as fixed amount]** — 當您想要以固定金額調整定義的[!DNL Commerce]價格來源值時，請選擇此選項。</li></ul> |
| [!UICONTROL Adjustment Amount] | 必填。<br><br>如果您選擇`Apply as percentage`作為&#x200B;*[!UICONTROL Apply]*，請輸入百分比值（例如：輸入`25`作為25%的百分比調整）。<br><br>如果您選擇`Apply as fixed amount`作為&#x200B;*[!UICONTROL Apply]*，請輸入固定金額的數值（例如：輸入`25`作為$25固定調整）。 |
