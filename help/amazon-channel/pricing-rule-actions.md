---
title: Amazon sales channel — 價格規則動作
description: 使用價格規則動作來定義套用至價格來源的調整計算，以決定Amazon的定價。
feature: Sales Channels, Price Rules
exl-id: c46bd5c2-7994-45b4-ae0c-9e473372c73a
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# 價格規則動作

價格規則作業會定義套用至價格來源的調整計算，以決定上市價格。

## 標準價格規則

A [標準價格規則](./standard-price-rules.md) Amazon可讓您以特定百分比或相對於 [!DNL Commerce] 型錄價格（或價格來源）。

| 章節 | 說明 |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./standard-price-rules.md) | 將規則型別設為 `Standard price rule`. |
| [[!UICONTROL Price Adjustment]](./standard-price-rules.md) | 定義套用至價格來源的調整計算，以決定清單價格 |

## 智慧型重新訂價規則

一個 [智慧型重新訂價規則](./intelligent-repricing-rules.md) 使用Amazon競爭者的定價來決定您的掛牌價格。 競爭對手是其他銷售商，列出與您在Amazon上列出的產品相同的產品。

| 章節 | 說明 |
|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md) | 將規則型別設為 `Intelligent repricing rule` 以及您的競爭者價格來源和意見反應需求。 |
| [[!UICONTROL Competitor Conditional Variances]](./competitor-conditional-variances.md) | 針對競爭對手銷售的相同產品定義條件差異。 |
| [[!UICONTROL Price Adjustment]](./price-adjustment.md) | 定義套用至價格來源的調整計算，以決定清單價格 |
| [[!UICONTROL Floor Price]](./floor-price.md) | 定義產品的最低價格，以防止多個定價規則將上市價格設定得太低。 |
| [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md) | 定義產品的最高價格，確保您的定價仍具競爭力。 |
