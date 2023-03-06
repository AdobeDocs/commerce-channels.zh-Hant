---
title: 「智慧重新定價規則：選擇規則類型
description: 建立智慧型重新定價規則，根據競爭者定價決定您的Amazon上市價格。
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# 智慧重新定價規則：選擇規則類型

>[!IMPORTANT]
>
>如果Amazon地區設為 `Inactive` 狀態，如上線期間。 貴機構的定價取決於運費，貴機構所在地區必須位於 `Active` 從Amazon同步的運費狀態。<br><br>
>
>若要更新Amazon帳戶中的地區狀態，請前往「設定>帳戶資訊>度假設定」。 請參閱 [Amazon:假期的清單狀態](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

智慧型重新定價規則會使用Amazon競爭者的定價來決定您的上市價格。 競爭者是在Amazon上列出與您相同產品的其他銷售者。

智慧重新定價規則的章節包括：

- 選擇規則類型
- [競爭者條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [最低價格](./floor-price.md)
- [可選最高價格](./optional-ceiling-price.md)

## 設定規則類型

在 _[!UICONTROL Select Rule Type]_區段。

1. 針對 **[!UICONTROL Rule Type]**，選擇 `Intelligent repricing rule`.

   此設定會啟用 _[!UICONTROL Competitor Price Source]_欄位和 [_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md), [_[!UICONTROL Floor Price]_](./floor-price.md)，和 [_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md) 區段。

1. 針對 **[!UICONTROL Competitor Price Source]**，選擇選項：

   - **[!UICONTROL Use "Buy Box" Price]**  — 選擇您要根據Amazon調整Amazon定價的時機 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 賣方價格。 A [!DNL Buy Box] 當Amazon上的多個銷售者提供相同產品時，即存在價格。 Amazon定義 [!DNL Buy Box] 賣方，根據表現要求。 商人想贏 [!DNL Buy Box] 銷售商狀態，並提供其產品清單的最大可見度。

   - **[!UICONTROL Use Lowest Competitor Price]**  — 選擇您想要比較和調整同一產品的上市價格與競爭者定價。 選擇後， _[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_ 欄位。

1. 如果已啟用，請為 **[!UICONTROL Minimum Positive Feedback]**.

   - **[!UICONTROL All Competitor's Prices]**  — 根據同一產品的所有競爭者價格，選擇您要比較和調整定價的時間。

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]**  — 選擇何時要限制與同一產品進行比較的競爭對手。 此設定要求其上市在適用最低價格規則之前，必須達到所選正反饋的最低百分比，從而進一步縮小競爭對手的範圍。

1. 如果已啟用，請輸入 **[!UICONTROL Minimum Feedback Count]**.

   此可選數值進一步縮小了競爭性定價。 例如，如果某個商戶有95%的正面意見評等，但只有意見計數為 `20`，您可能不想針對此修改定價。 不過，如果您輸入 `1000`這將要求商家有95%的正面反饋，至少有1000個商家評論。

>[!NOTE]
>
>您可以使用這些競爭者定價和反饋選項，來避免根據反饋不佳且銷售質量較低的產品的競爭對手來進行定價。

![智慧重新定價規則 — 選擇規則類型](assets/ob-intelligent-price-rule-type.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Rule Type] | 選取規則類型。 選項：<ul><li>**[!UICONTROL Standard price rule]**  — 此規則類型可讓您以特定百分比或固定金額，相對於 _[!UICONTROL Magento Price Source]_. </li><li>**[!UICONTROL Intelligent repricing rule]**  — 此規則類型可讓您根據競爭者的定價調整Amazon上市價格。 選擇後， _[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_ 欄位。</li></ul> |
| [!UICONTROL Competitor Price Source] | 選擇所需的價格來源。 選項：<ul><li>**[!UICONTROL Use "Buy Box" Price]**  — 當您要根據Amazon調整Amazon定價時，請選擇此選項 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 賣方價格。 A [!DNL Buy Box] 當Amazon上的多個銷售者提供相同產品時，即存在價格。 Amazon定義 [!DNL Buy Box] 賣方，根據表現要求。 商人想贏 [!DNL Buy Box] 銷售商狀態，並提供其產品清單的最大可見度。</li><li>**[!UICONTROL Use Lowest Competitor Price]**  — 當您想要比較並調整您的上市價格，並將其調整為 [最低競爭者定價](./lowest-competitor-pricing.md) 相同產品。 選擇後， _[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_ 欄位。</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | 只有在 `Use Lowest Competitor Price` 已選取。 選項：<ul><li>**[!UICONTROL All Competitor's Prices]**  — 根據同一產品的所有競爭者價格，選擇您要比較和調整定價的時間。</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]**  — 選擇您要限制比較的競爭對手的時間並調整定價。 此設定會進一步縮小您的競爭者，要求其上市必須達到所選正反饋的最低百分比，然後使用該競爭者子集的最低價格。</li></ul> |
| [!UICONTROL Minimum Feedback Count] | 只有在 `Use Lowest Competitor Price` 已選取。 此可選數值進一步縮小了競爭性定價比較。 例如，如果某個商戶有95%的正反饋評分，但只有反饋計數為 `20`，您可能不想針對此修改定價。 不過，如果您輸入 `1000`這將要求商家有95%的正面反饋，至少有1000個商家評論。 |
