---
title: 建立 [!DNL Commerce] Amazon屬性
description: 在完成Amazon銷售渠道登錄過程之前，請確保您有必要 [!UICONTROL Commerce] 產品屬性。
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 建立 [!DNL Commerce] Amazon屬性

在登機前 [!DNL Amazon Seller Central] 帳戶，這是添加 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"} 映射產品清單。 完成登錄後，您可以通過 [屬性](./managing-attributes.md) 頁籤 [Amazon銷售渠道首頁](./amazon-sales-channel-home.md) 的子菜單。

這些說明詳細說明了如何建立 [!DNL Commerce] 屬性。 建議建立包括AmazonEAN、AmazonISBN和AmazonUPC在內的其他屬性。 如果您想將Amazon上市價格用作定價規則的價格來源，則可能還要建立「Amazon價格」屬性。 這些屬性用於在入門期間配置清單和定價設定。 在建立Amazon清單以及更新和同步您的清單時，也使用這些屬性 [!DNL Commerce] 你的Amazon目錄。

「目錄搜索」設定允許您設定匹配的搜索參數，以幫助映射符合條件的 [!DNL Commerce] Amazon上市的產品。 映射後，Amazon將激活與定價、數量、改寫以及訂單和產品同步相關的操作。

定義這些值會增加精確匹配的可能性，從而最大限度地減少以後手動匹配產品清單的需要。 添加屬性作為登錄的一部分 [預設定任務](./amazon-pre-setup-tasks.md),Amazon銷售渠道在Amazon與 [!DNL Commerce] 一次性的。

如果僅建立AmazonASIN屬性（不為每個產品添加ASIN值），則 [!DNL Commerce] 產品可能不會自動與您的Amazon清單匹配。 您可以通過 _儲存審閱_。 但是，手動匹配不會建立共用和同步產品資料所需的資料元素。

>[!IMPORTANT]
>
>如果為手動匹配的產品更新ASIN、UPC或其他資料元素，則必須在以下兩個位置更新資料：你 [!DNL Commerce] 目錄和清單 [!DNL Amazon Seller Central] 帳戶。

## 建立AmazonASIN產品屬性

1. 登錄 [!DNL Commerce] 管理員。

1. 按一下 **[!UICONTROL Stores]** 的上界。

1. 在 _[!UICONTROL Attributes]_，按一下&#x200B;**[!UICONTROL Product]**。

1. 要開啟屬性屬性，請按一下 **[!UICONTROL Add New Attribute]**。

1. 對於 **[!UICONTROL Default Label]**&#x200B;輸入 `Amazon ASIN` （屬性的名稱）。

1. 對於 **[!UICONTROL Catalog Input Type for Store Owner]**&#x200B;選項 `Text Field`。

1. 對於 **[!UICONTROL Values Required]**&#x200B;選項 `No`。

   雖然AmazonASIN需要在Amazon上列出產品，但您的某些目錄產品可能未在Amazon上列出。

1. 展開 _[!UICONTROL Advanced Attribute Properties]_，並設定選項：

   - 對於 **[!UICONTROL Attribute Code]**&#x200B;輸入 `amazon_asin`。

   - 對於 **[!UICONTROL Scope]**&#x200B;選項 `Global`。

   - 對於 **[!UICONTROL Unique Value]**&#x200B;選項 `No`。

   - 對於 **[!UICONTROL Input Validation for Store Owner]**&#x200B;選項 `None`。

   - 對於 **[!UICONTROL Add to Column Options]**&#x200B;選項 `Yes`。

   - 對於 **[!UICONTROL Use in Filter Options]**&#x200B;選項 `Yes`。

1. 按一下 **[!UICONTROL Save Attribute]**。

![AmazonASIN屬性](assets/creating-asin-attribute.png)

## 建立Amazon條件產品屬性

1. 登錄 [!DNL Commerce] 管理員。

1. 按一下 **[!UICONTROL Stores]** 的上界。

1. 在 _[!UICONTROL Attributes]_，按一下&#x200B;**[!UICONTROL Product]**。

1. 要開啟屬性屬性，請按一下 **[!UICONTROL Add New Attribute]**。

1. 對於 **[!UICONTROL Default Label]**&#x200B;輸入 `Amazon Condition` （屬性的名稱）。

1. 對於 **[!UICONTROL Catalog Input Type for Store Owner]**&#x200B;選項 `Dropdown`。

   的 _[!UICONTROL Manage Options (Values of your Attribute)]_的上界。

1. 對於 **[!UICONTROL Values Required]**&#x200B;選項 `No`。

1. 對於 **[!UICONTROL Manage Options (Values for your Attribute)]**，添加每個條件選項。

   標準Amazon條件包括：

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. 按一下 **[!UICONTROL Add Option]**。

1. 選擇 **[!UICONTROL Is Default]** 頁籤

1. 在 _[!UICONTROL Admin]_列中，輸入要添加條件的標籤的文本(例如 `New`。 `Used`, `Used-Like New`)

1. 按一下 **[!UICONTROL Add Option]** 以根據需要添加更多選項。

1. 展開 _[!UICONTROL Advanced Attribute Properties]_的子菜單。

   - 對於 **[!UICONTROL Attribute Code]**&#x200B;輸入 `amazon_condition`。

   - 對於 **[!UICONTROL Scope]**&#x200B;選項 `Global`。

   - 對於 **[!UICONTROL Unique Value]**&#x200B;選項 `No`。

   - 對於 **[!UICONTROL Input Validation for Store Owner]**&#x200B;選項 `None`。

   - 對於 **[!UICONTROL Add to Column Options]**&#x200B;選項 `Yes`。

   - 對於 **[!UICONTROL Use in Filter Options]**&#x200B;選項 `Yes`。

1. 按一下 **[!UICONTROL Save Attribute]**。

![Amazon條件屬性](assets/creating-amazon-condition-attribute.png)

![下一個表徵圖](assets/btn-next.png) [**繼續添加或驗證API密鑰**](./amazon-verify-api-key.md)
