---
title: 管理Amazon定價
description: 您可以使用定價規則將Amazon清單的定價設定為與您的電子商務商店不同。
redirect_from: /sales-channels/asc/ob-pricing-rules.html
exl-id: 5c990206-ac72-4ef5-9ed0-ff8d816096eb
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# 管理Amazon定價

Amazon銷售渠道允許您設定定價規則，這允許您設定與定義的Amazon上市價格不同的定價 **[!UICONTROL Magento Price Source]** 在 [上市價格](./listing-price.md)。 您還可以堆疊多個規則，甚至可以使用智慧定價根據競爭對手的產品調整您的Amazon上市價格 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 價格或 [最低競爭對手價格](./lowest-competitor-pricing.md)。

定價規則有兩種類型：

- [標準定價規則](./standard-price-rules.md)
- [智慧重定價規則](./intelligent-repricing-rules.md)

   >[!IMPORTANT]
   >
   >如果將Amazon區域設定為，智慧重定價規則無法正常運行 `Inactive` 狀態，就像登機時一樣。 您的定價計算取決於發運費率，並且您的區域必須位於 `Active` 要從Amazon同步的裝運費率的狀態。
   >
   >要更新Amazon帳戶中的區域狀態，請轉至「設定」>「帳戶資訊」>「假期設定」。 請參閱 [Amazon:列出假期狀態](https://sellercentral.amazon.com/gp/help/help.html?itemID=200135620){target="_blank"} （需要賣方中心登錄）。

此功能允許您以類似於 [!DNL Commerce] [目錄價格規則](https://docs.magento.com/user-guide/catalog/pricing.html){target="_blank"}。 您可以建立複雜規則，以便更改特定產品、特定類別內的產品或甚至具有特定屬性的價格。

您可以為您的Amazon清單添加定價規則。 價格規則可用於根據一組定義的條件自動調整您的上市價格。 在產品在Amazon上市之前，系統會觸發價格規則並計算調整後的價格。

>[!NOTE]
>
>您的Amazon清單的價格來源是 **[!UICONTROL Magento Price Source]** 在 [上市價格](./listing-price.md) 的子菜單。 在定價規則中定義的任何調整計算都使用價格來源作為起始值。

定價規則允許您將Amazon上市價格設定為與 **[!UICONTROL Magento Price Source]** 在 [上市價格](./listing-price.md) 的子菜單。 您還可以堆疊多個規則，這些規則可以協同工作來調整價格。

定價/重新定價規則在設定過程中需要三組資訊：

- [常規設定](./pricing-rule-general-settings.md):定義規則的名稱、說明、活動日期、優先順序，並基於其優先順序設定設定後續規則的行為。
- [條件](./pricing-rule-conditions.md):確定哪些產品符合價格規則。
- [操作](./pricing-rule-actions.md):定義應用於價格來源以確定上市價格的調整計算。

您可以建立 [標準定價規則](./standard-price-rules.md) 自動調整您的Amazon上市價格 **[!UICONTROL Magento Price Source]** 在 [上市價格](./listing-price.md) 的子菜單。 此功能允許您以類似於 [!DNL Commerce] [目錄價格規則](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"}。 您可以建立複雜規則，自動更改特定產品、特定類別內的產品或具有特定屬性的產品的價格。 您可以完成傳統設定並根據固定金額或百分比對產品重新定價以增加或減少。

另一個強大的工具是 [智慧重定價](./intelligent-repricing-rules.md) 功能根據競爭對手調整您的Amazon上市價格 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 價格或 [最低競爭對手價格](./lowest-competitor-pricing.md)。 與 [!DNL Commerce] [目錄價格規則](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"}，此高級功能允許您通過建立複雜規則來操縱Amazon價格。 規則可以定義特定產品、特定類別內的產品或甚至具有特定產品屬性的價格更改範圍。

使用智慧重新定價根據競爭對手的定價調整您的Amazon上市價格。 Amazon銷售渠道已為您內置保護措施，您可以配置以保護利潤率或避免將商家的價格與低反饋相匹配。 使用 [智慧重定價規則](./intelligent-repricing-rules.md),Amazon的上市價格可以自動被操縱為固定或百分比金額（上下），甚至與 [[!DNL Buy Box]](./buy-box-competitor-pricing.md) 價格或 [最低競爭對手價格](./lowest-competitor-pricing.md) 按每個項目計算。 規則甚至可以堆疊起來提供無限的靈活性。

您可以控制規則的重要方面，如活動/非活動狀態、網站資格、可選日期範圍和可選優先順序（用於規則堆疊）。

例如，您可以定義和設定價格規則的條件，在滿足這些條件後，在將其發送到Amazon之前，將自動調整您的上市價格。

另一個定價選項是 [價格覆蓋](./overrides.md)，在個別清單層設定。 A [價格覆蓋](./overrides.md) 可以設定，覆蓋忽略/優先於所有其他預設值、設定和規則。 安 [覆蓋](./overrides.md) 可以為價格、處理時間、條件和銷售者附註設定（少數例外）。

![定價規則](assets/amazon-pricing-rules.png)

## 預設列

| 列 | 說明 |
|---|---|
| [!UICONTROL Name] | 定價規則的名稱，如中所設定 [定價規則常規設定](./pricing-rule-general-settings.md) |
| [!UICONTROL Rule Type] | 規則類型，如中所設定 [定價規則操作](./pricing-rule-actions.md) （標準價格規則或智慧重新定價規則） |
| [!UICONTROL Is Active] | 規則是否處於活動狀態，如中所設定 [定價規則常規設定](./pricing-rule-general-settings.md) |
| [!UICONTROL Priority] | 優先於其他定價條件（如中所設定） [定價規則常規設定](./pricing-rule-general-settings.md) |
| [!UICONTROL Stop Further Rules Processing] | 指示是否對符合此規則的產品進一步處理價格規則，如中所設定 [定價規則常規設定](./pricing-rule-general-settings.md) |
| [!UICONTROL From Date] | 規則處於活動狀態的時段的開始 |
| [!UICONTROL To Date] | 規則處於活動狀態的時段的結束 |
| [!UICONTROL Action] | 列出可應用於特定清單的所有操作。 要應用操作，請按一下 **[!UICONTROL Select]** 的 _[!UICONTROL Action]_的雙曲餘切值。 選項： `Edit Price Rule` / `Delete Price Rule` |
