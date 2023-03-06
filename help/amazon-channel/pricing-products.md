---
title: 管理Amazon定價
description: 您可以使用定價規則，將Amazon清單的定價設為與CoMerce Store不同。
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# 管理Amazon定價

Amazon銷售管道可讓您設定定價規則，以便您設定與已定義之不同的Amazon上市價格 **[!UICONTROL Magento Price Source]** 在 [上市價](./listing-price.md). 您也可以堆疊多個規則，甚至使用智慧型定價，根據競爭者的 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 價格或 [競爭者價格](./lowest-competitor-pricing.md).

定價規則有兩種類型：

- [標準定價規則](./standard-price-rules.md)
- [智慧重新定價規則](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >如果Amazon地區設為 `Inactive` 狀態，如上線期間。 貴機構的定價取決於運費，貴機構所在地區必須位於 `Active` 從Amazon同步的運費狀態。
   >
   >若要更新Amazon帳戶中的地區狀態，請前往「設定>帳戶資訊>度假設定」。 請參閱 [Amazon:假期的清單狀態](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){target="_blank"} （需要賣方中心登錄）。

此功能可讓您以類似以下的方式操控Amazon價格： [!DNL Commerce] [目錄價格規則](https://docs.magento.com/user-guide/catalog/pricing.html){target="_blank"}. 您可以建立複雜規則，以便變更特定產品、特定類別內的產品或甚至特定屬性的價格。

您可以為Amazon清單新增定價規則。 價格規則可用來根據一組已定義的條件自動調整您的上市價格。 在產品於Amazon上市前，系統會觸發價格規則並計算您調整後的價格。

>[!NOTE]
>
>Amazon清單的價格來源是 **[!UICONTROL Magento Price Source]** 在 [上市價](./listing-price.md) 設定。 定價規則中定義的任何調整計算都使用價格來源作為起始值。

定價規則可讓您將Amazon的上市價格設為與 **[!UICONTROL Magento Price Source]** 在 [上市價](./listing-price.md) 設定。 您也可以堆疊多個可搭配運作的規則，以調整價格。

定價/重新定價規則設定期間需要三組資訊：

- [一般設定](./pricing-rule-general-settings.md):定義規則的名稱、說明、作用中日期、優先順序，並根據其優先順序設定後續規則的行為。
- [條件](./pricing-rule-conditions.md):確定哪些產品符合價格規則。
- [動作](./pricing-rule-actions.md):定義應用於價格來源以確定上市價格的調整計算。

您可以建立 [標準定價規則](./standard-price-rules.md) 會自動調整您Amazon的上市價格， **[!UICONTROL Magento Price Source]** 在 [上市價](./listing-price.md) 設定。 此功能可讓您以類似以下的方式操控Amazon價格： [!DNL Commerce] [目錄價格規則](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"}. 您可以建立複雜的規則，自動更改特定產品、特定類別內的產品或具有特定屬性的產品的價格。 您可以完成傳統設定，並根據固定金額或百分比重新定價產品以增加或減少。

另一個強大的工具是 [智慧重新定價](./intelligent-repricing-rules.md) 功能，可根據競爭者調整您的Amazon上市價格 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 價格或 [競爭者最低價格](./lowest-competitor-pricing.md). 類似於 [!DNL Commerce] [目錄價格規則](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"}，此進階功能可讓您建立複雜規則來控制Amazon價格。 規則可以定義特定產品、特定類別內的產品，甚至特定產品屬性的價格變更範圍。

根據競爭者的定價，使用智慧重新定價來調整您的Amazon上市價格。 Amazon銷售管道已為您內建保護機制，可讓您進行設定以保護利潤率，或避免將商家的價格與低反饋配對。 使用 [智慧重定價規則](./intelligent-repricing-rules.md),Amazon的清單價格可自動以固定或百分比金額（向上或向下）操控，或甚至同步至 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 價格或 [競爭者最低價格](./lowest-competitor-pricing.md) 按每個項目計算。 規則甚至可堆疊，以提供無限的彈性。

您可以控制規則的重要方面，例如作用中/非作用中狀態、網站資格、可選日期範圍和可選優先順序層級（用於規則堆疊）。

例如，您可以定義並設定價格規則的條件，當符合條件時，系統會自動調整您的上市價格，再將其傳送至Amazon。

另一個定價選項是 [價格覆蓋](./overrides.md)，而此會在個別清單層級設定。 A [價格覆蓋](./overrides.md) 可以設定，且覆寫會忽略/優先順序高於所有其他預設值、設定和規則。 安 [覆寫](./overrides.md) 可針對價格、處理時間、條件和賣方附註進行設定（少數例外）。

![定價規則](assets/amazon-pricing-rules.png)

## 預設列

| 欄 | 說明 |
|---|---|
| [!UICONTROL Name] | 定價規則的名稱，如 [定價規則一般設定](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | 規則類型，如 [定價規則動作](./pricing-rule-actions.md) （標準價格規則或智慧重新定價規則） |
| [!UICONTROL Is Active] | 規則是否為作用中，如 [定價規則一般設定](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | 優先順序高於其他定價條件，如 [定價規則一般設定](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | 指出是否對符合此規則的產品處理任何進一步的價格規則，如 [定價規則一般設定](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | 規則生效的時段的開頭 |
| [!UICONTROL To Date] | 規則作用中時段的結尾 |
| [!UICONTROL Action] | 列出可套用至特定清單的所有動作。 若要套用動作，請按一下 **[!UICONTROL Select]** 在 _[!UICONTROL Action]_欄。 選項： `Edit Price Rule` / `Delete Price Rule` |
