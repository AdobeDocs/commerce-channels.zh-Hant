---
title: 「智慧重定價規則：選擇規則類型
description: 通過建立智慧重新定價規則，根據競爭對手定價確定您的Amazon上市價格。
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# 智慧重定價規則：選擇規則類型

>[!IMPORTANT]
>
>如果將Amazon區域設定為，智慧重定價規則無法正常運行 `Inactive` 狀態，就像登機時一樣。 您的定價計算取決於發運費率，並且您的區域必須位於 `Active` 要從Amazon同步的裝運費率的狀態。<br><br>
>
>要更新Amazon帳戶中的區域狀態，請轉至「設定」>「帳戶資訊」>「假期設定」。 請參閱 [Amazon:列出假期狀態](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

智慧的重新定價規則使用Amazon競爭對手的定價來確定您的上市價格。 競爭對手是其他銷售商，他們在Amazon上列出了與您相同的產品。

智慧重新定價規則的部分包括：

- 選擇規則類型
- [競爭對手條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [底價](./floor-price.md)
- [可選上限價格](./optional-ceiling-price.md)

## 配置規則類型

在中定義規則類型 _[!UICONTROL Select Rule Type]_的子菜單。

1. 對於 **[!UICONTROL Rule Type]**&#x200B;選項 `Intelligent repricing rule`。

   此設定啟用 _[!UICONTROL Competitor Price Source]_的 [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md)。 [_[!UICONTROL Floor Price]_](./floor-price.md), [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) 的下界。

1. 對於 **[!UICONTROL Competitor Price Source]**，選擇選項：

   - **[!UICONTROL Use "Buy Box" Price]**  — 選擇何時根據Amazon調整Amazon定價 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 賣方價格。 A [!DNL Buy Box] 當Amazon的多個賣家提供同一產品時，價格就存在。 Amazon定義 [!DNL Buy Box] 賣方的合約。 商人爭取 [!DNL Buy Box] 銷售商狀態，並提供其產品清單的最大可視性。

   - **[!UICONTROL Use Lowest Competitor Price]**  — 選擇要比較和調整清單價格與同一產品的競爭對手定價的時間。 選擇後， _[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_ 欄位。

1. 如果啟用，請為 **[!UICONTROL Minimum Positive Feedback]**。

   - **[!UICONTROL All Competitor's Prices]**  — 根據同一產品的所有競爭對手價格，選擇要比較和調整定價的時間。

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]**  — 選擇您希望限制與同一產品的價格進行比較的競爭對手的時間。 此設定要求競爭對手在應用最低價格規則之前具有所選正反饋百分比的最小值，從而進一步縮小了競爭對手的範圍。

1. 如果啟用，請為 **[!UICONTROL Minimum Feedback Count]**。

   這一可選數值進一步縮小了競爭性定價的範圍。 例如，如果某商戶具有95%的正反饋評級，但僅具有以下反饋計數： `20`，它可能不是您要修改定價的競爭對手。 但是，如果輸入的值 `1000`它要求商戶有95%的正面反饋和至少1000個商戶評論。

>[!NOTE]
>
>您可能會使用這些競爭對手的定價和反饋選項，以避免根據反饋較差且銷售質量較低產品的競爭對手進行定價。

![智慧重定價規則 — 選擇規則類型](assets/ob-intelligent-price-rule-type.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Rule Type] | 選擇規則類型。 選項：<ul><li>**[!UICONTROL Standard price rule]**  — 此規則類型允許您將Amazon上市價格相對於 _[!UICONTROL Magento Price Source]_。 </li><li>**[!UICONTROL Intelligent repricing rule]**  — 此規則類型允許您根據競爭對手的定價調整Amazon上市價格。 選擇後， _[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_ 欄位。</li></ul> |
| [!UICONTROL Competitor Price Source] | 選擇所需的價格來源。 選項：<ul><li>**[!UICONTROL Use "Buy Box" Price]**  — 當您要根據Amazon調整Amazon定價時，請選擇此選項 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 賣方價格。 A [!DNL Buy Box] 當Amazon的多個賣家提供同一產品時，價格就存在。 Amazon定義 [!DNL Buy Box] 賣方的合約。 商人爭取 [!DNL Buy Box] 銷售商狀態，並提供其產品清單的最大可視性。</li><li>**[!UICONTROL Use Lowest Competitor Price]**  — 當要將清單價格與 [最低競爭對手定價](./lowest-competitor-pricing.md) 同一產品。 選擇後， _[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_ 欄位。</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | 僅當 `Use Lowest Competitor Price` 的子菜單。 選項：<ul><li>**[!UICONTROL All Competitor's Prices]**  — 根據同一產品的所有競爭對手價格，選擇要比較和調整定價的時間。</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]**  — 選擇希望限制您比較的競爭對手並調整定價的時間。 此設定要求其上市必須具有所選正反饋百分比的最小值，然後使用該子集競爭對手的最低價格，從而進一步縮小了競爭對手的範圍。</li></ul> |
| [!UICONTROL Minimum Feedback Count] | 僅當 `Use Lowest Competitor Price` 的子菜單。 這一可選數值進一步縮小了競爭性定價比較的範圍。 例如，如果某商戶具有95%的正反饋評級，但僅具有以下反饋計數 `20`，它可能不是您要修改定價的競爭對手。 但是，如果輸入的值 `1000`它要求商戶有95%的正面反饋和至少1000個商戶評論。 |
