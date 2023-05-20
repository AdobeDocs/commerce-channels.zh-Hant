---
title: 「智慧重定價規則：競爭對手條件差異
description: 通過建立智慧重定價規則，根據競爭對手的定價和產品狀況確定您的Amazon上市價格。
exl-id: c52230e3-4e47-45bc-80e0-170530f58987
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 智慧重定價規則：競爭對手條件差異

智慧重新定價規則的部分包括：

- [[!UICONTROL Select Rule Type]](./intelligent-repricing-rules.md)
- [!UICONTROL Competitor Conditional Variances]
- [[!UICONTROL Price Adjustment]](./price-adjustment.md)
- [[!UICONTROL Floor Price]](./floor-price.md)
- [[!UICONTROL Optional Ceiling Price]](./optional-ceiling-price.md)

智慧的重新定價規則使用Amazon競爭對手的定價來確定您的上市價格。 競爭對手是其他銷售商，它們正在上市的產品與你在Amazon上市的產品相同。

如果存在具有相同條件的產品，則基本匹配價格為 [最差競爭對手](./lowest-competitor-pricing.md) 同等條件的價格。 如果沒有競爭對手的產品與您的條件匹配，則基本匹配價格將通過其他可用競爭對手的條件（從「新建」、「翻新」和「繼續」到可用條件）。 找到條件後，基本匹配價格將是該條件內的最低價格。

如果您的產品列有條件 `Used; Good` 基準匹配價格，競爭者在相同條件下以較低價格使用相同產品，則使用競爭者價格。 如果競爭對手不存在相同的條件，系統將檢查具有下一個條件的競爭對手， `New`。 如果發現競爭對手具有該條件，則使用最低價格。

## 配置競爭對手的條件差異

在 _[!UICONTROL Competitor Conditional Variances]_的子菜單。

對於 **[!UICONTROL Conditional Variance]**，選擇選項：

- `Use all competitor's product conditions`  — （預設）選擇希望產品與任何可用條件進行比較的時間（如果所列條件不存在匹配項）。

- `Use Only Matching Competitor's Product Condition`  — 選擇希望您的產品只與處於相同條件的競爭對手的產品進行比較的時間。 如果不存在匹配項，則產品將按 _Magento價格來源_ 定義 [上市價格](./listing-price.md)。

- `Apply Variance (if competitor's product condition differs)`  — 選擇首先嘗試與匹配的產品條件進行比較。 如果不存在匹配條件，則會對您的產品條件和最低競爭對手的條件應用差異（以百分比表示）。

   當 _[!UICONTROL Apply Variance]_選擇功能，將顯示每個Amazon條件的附加方差欄位。 此功能允許您在提供與競爭對手處於不同狀態的產品時使用智慧重新定價規則。 要瞭解條件差異背後的計算，您必須首先瞭解所有差異都是根據基本匹配價格確定的。

   出現的條件差異選項基於清單設定 `Condition` 使用 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}。 對於所有映射的條件，可以定義1-100的方差百分比。 例外是可收集的，在這種情況下，可應用大於100的百分比。

![智慧重定價規則 — 競爭對手條件差異](assets/amazon-competitor-cond-variances.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Competitor Conditional Variances] | 選項： <ul><li>**[!UICONTROL Use all competitor's product conditions]**  — 如果所列產品的條件不存在匹配項，則此選項與任何可用條件匹配。 它首先嘗試匹配您的狀況，然後從 `New` 條件 `Used; Acceptable`。</li><li>**[!UICONTROL Use only matching competitor's product condition]**  — 此選項與您產品的條件匹配。 如果不存在匹配，則 _[!UICONTROL Magento Price Source]_。</li><li>>**[!UICONTROL Apply variance (if competitor's product condition differs)]**  — 此選項首先嘗試與您的產品條件匹配。 如果不存在匹配條件，則它將應用與您的產品條件和最低競爭對手的條件相關的差異（以百分比表示）。</li></ul><br><br>根據條件清單設定顯示的條件差異選項，這些條件差異選項使用 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html){target="_blank"}。 對於所有映射的條件，可以表示1-100的方差百分比。 例外是可收集的，在這種情況下，可應用大於100的百分比。<br><br>此功能允許您在提供與競爭對手處於不同狀態的產品時使用智慧重新定價規則。 要瞭解條件差異背後的計算，您必須首先瞭解所有差異都是根據基本匹配價格確定的。 |

## 計算條件方差基

- 基本匹配條件差異(BMC)=基本匹配價格競爭對手的條件差異。 使用前面的示例，BMC是 `New` 的子菜單。
- 商家條件差異(MCV)=產品條件的差異。 使用前例，MCV = `Used; Good` 的子菜單。
- 基本匹配價格(BMP)= 7.99美元（上面說明）

計算條件方差基數的公式如下：

![條件方差基計算公式](assets/amazon-cond-variance-calc-1.png)

## 示例

條件差異設定如下：

![示例條件差異設定](assets/amazon-cond-variances.png)

- BMC = 100（競爭對手條件=新建）
- MCV = 80(商家條件=已用；好)
- BMP = 7.99美元（基本匹配價格=匹配競爭對手條件的最低價格）

![條件方差基計算示例](assets/amazon-cond-variance-calc-2.png)

使用上面的條件差異基數計算，條件差異基數= $6.39。此計算是用於價格規則活動的競爭對手價格來源，詳見 [價格調整](./price-adjustment.md)。
