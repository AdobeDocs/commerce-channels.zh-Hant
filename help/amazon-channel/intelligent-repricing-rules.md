---
title: 「智慧重新定價規則：選擇規則類型
description: 建立智慧型重新定價規則，根據競爭者定價決定您的Amazon上市價格。
exl-id: 2690323a-a076-484b-a437-adadb08094f5
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# 智慧重新定價規則：選擇規則類型

>[!IMPORTANT]
>
>如果Amazon地區設為`Inactive`狀態（如上線期間），智慧型重新定價規則將無法正常運作。 您的定價計算取決於您的運費，且您的地區必須處於`Active`狀態，您的運費才能從Amazon同步。<br><br>
>
>若要更新Amazon帳戶中的地區狀態，請前往「設定>帳戶資訊>度假設定」。 請參閱[Amazon:假期的清單狀態](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620/&quot;target=&quot;_blank)

智慧型重新定價規則會使用Amazon競爭者的定價來決定您的上市價格。 競爭者是在Amazon上列出與您相同產品的其他銷售者。

智慧重新定價規則的章節包括：

- 選擇規則類型
- [競爭者條件差異](./competitor-conditional-variances.md)
- [價格調整](./price-adjustment.md)
- [最低價格](./floor-price.md)
- [可選最高價格](./optional-ceiling-price.md)

## 設定規則類型

在&#x200B;_[!UICONTROL Select Rule Type]_區段中定義規則類型。

1. 對於&#x200B;**[!UICONTROL Rule Type]**，選擇`Intelligent repricing rule`。

   此設定可啟用&#x200B;_[!UICONTROL Competitor Price Source]_欄位以及[_[!UICONTROL Competitor Conditional Variances]_](./competitor-conditional-variances.md)、[_[!UICONTROL Floor Price]_](./floor-price.md)和[_[!UICONTROL Optional Ceiling Price]_](./optional-ceiling-price.md)區段。

1. 對於&#x200B;**[!UICONTROL Competitor Price Source]**，選擇一個選項：

   - **[!UICONTROL Use "Buy Box" Price]**  — 根據Amazon賣方價格選擇您要調整Amazon定價 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 的時間。當Amazon上的多個銷售者提供相同產品時，即存在[!DNL Buy Box]價格。 Amazon根據業績要求定義[!DNL Buy Box]賣方。 商家尋求獲得[!DNL Buy Box]賣方狀態，並提供其產品清單的最大可見性。

   - **[!UICONTROL Use Lowest Competitor Price]**  — 選擇您想要比較和調整同一產品的上市價格與競爭者定價。選擇後，將啟用&#x200B;_[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_&#x200B;欄位。

1. 如果已啟用，請為&#x200B;**[!UICONTROL Minimum Positive Feedback]**&#x200B;選擇一個選項。

   - **[!UICONTROL All Competitor's Prices]**  — 根據同一產品的所有競爭者價格，選擇您要比較和調整定價的時間。

   - **[!UICONTROL Minimum 80/90/95/98% positive feedback]**  — 選擇何時要限制與同一產品進行比較的競爭對手。此設定要求其上市在適用最低價格規則之前，必須達到所選正反饋的最低百分比，從而進一步縮小競爭對手的範圍。

1. 如果已啟用，請為&#x200B;**[!UICONTROL Minimum Feedback Count]**&#x200B;輸入數值。

   此可選數值進一步縮小了競爭性定價。 例如，如果某個商家的反饋評級為95%，但反饋計數為`20`，則它可能不是您要根據修改定價的競爭對手。 但是，如果輸入`1000`值，則要求商家有95%的正反饋，並且至少有1000個商家評論。

>[!NOTE]
>
>您可以使用這些競爭者定價和反饋選項，來避免根據反饋不佳且銷售質量較低的產品的競爭對手來進行定價。

![智慧重新定價規則 — 選擇規則類型](assets/ob-intelligent-price-rule-type.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Rule Type] | 選取規則類型。 選項：<ul><li>**[!UICONTROL Standard price rule]**  — 此規則類型可讓您以相對於的特定百分比或固定美元金額，來增加或減少Amazon上市價 _[!UICONTROL Magento Price Source]_格。 </li><li>**[!UICONTROL Intelligent repricing rule]**  — 此規則類型可讓您根據競爭者的定價調整Amazon上市價格。選擇後，將啟用&#x200B;_[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_&#x200B;欄位。</li></ul> |
| [!UICONTROL Competitor Price Source] | 選擇所需的價格來源。 選項：<ul><li>**[!UICONTROL Use "Buy Box" Price]**  — 當您要根據Amazon賣方價格調整Amazon定價時，請選 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 擇此選項。當Amazon上的多個銷售者提供相同產品時，即存在[!DNL Buy Box]價格。 Amazon根據業績要求定義[!DNL Buy Box]賣方。 商家尋求獲得[!DNL Buy Box]賣方狀態，並提供其產品清單的最大可見性。</li><li>**[!UICONTROL Use Lowest Competitor Price]**  — 當您想要比較並調整上市價格，使同一產品的競 [爭者](./lowest-competitor-pricing.md) 價格最低時，請選擇此選項。選擇後，將啟用&#x200B;_[!UICONTROL Minimum Positive Feedback]_和_[!UICONTROL Minimum Feedback Count]_&#x200B;欄位。</li></ul> |
| [!UICONTROL Minimum Positive Feedback] | 只有在選擇`Use Lowest Competitor Price`時才處於活動狀態。 選項：<ul><li>**[!UICONTROL All Competitor's Prices]**  — 根據同一產品的所有競爭者價格，選擇您要比較和調整定價的時間。</li><li>**[!UICONTROL Minimum 80/90/95/98% positive feedback]**  — 選擇您要限制比較的競爭對手的時間並調整定價。此設定會進一步縮小您的競爭者，要求其上市必須達到所選正反饋的最低百分比，然後使用該競爭者子集的最低價格。</li></ul> |
| [!UICONTROL Minimum Feedback Count] | 只有在選擇`Use Lowest Competitor Price`時才處於活動狀態。 此可選數值進一步縮小了競爭性定價比較。 例如，如果某個商家的反饋評級為95%，但反饋計數為`20`，則它可能不是您要根據修改定價的競爭對手。 但是，如果輸入`1000`值，則要求商家有95%的正反饋，並且至少有1000個商家評論。 |
