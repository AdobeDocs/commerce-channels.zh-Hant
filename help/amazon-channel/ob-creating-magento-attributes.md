---
title: 建立 [!DNL Commerce] Amazon屬性
description: 完成Amazon銷售管道入門程式之前，請確定您具備所需 [!UICONTROL Commerce] 產品屬性。
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 建立 [!DNL Commerce] Amazon屬性

開始使用 [!DNL Amazon Seller Central] 帳戶，則最佳作法是新增 [!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"} 來對應您的產品清單。 完成上線後，您可以透過 [屬性](./managing-attributes.md) 的 [Amazon銷售頻道首頁](./amazon-sales-channel-home.md) 頁面。

這些指示詳細說明如何建立 [!DNL Commerce] Amazon ASIN和Amazon條件的屬性。 建議建立其他屬性，包括Amazon EAN、Amazon ISBN和Amazon UPC。 如果您想要使用Amazon上市價格作為定價規則的價格來源，也可以建立Amazon價格屬性。 在上線期間設定清單和定價設定時，會使用這些屬性。 建立Amazon清單以及更新和同步您的 [!DNL Commerce] 目錄與您的Amazon清單。

「目錄搜尋」設定可讓您設定符合條件的搜尋參數，以利對應符合條件 [!DNL Commerce] 具有Amazon清單的產品。 映射後，Amazon將激活與定價、數量、改寫、訂單和產品同步相關的操作。

定義這些值會增加完全相符的可能性，將日後手動比對產品清單的需求降至最低。 新增屬性作為入門的一部分 [預先設定任務](./amazon-pre-setup-tasks.md),Amazon銷售管道在Amazon和 [!DNL Commerce] 上線後。

如果您僅建立Amazon ASIN屬性（不為每個產品新增ASIN值），則您的 [!DNL Commerce] 產品可能不會自動符合您的Amazon清單。 您可以透過 _商店審核_. 不過，手動比對不會建立共用及同步產品資料所需的資料元素。

>[!IMPORTANT]
>
>如果您更新了手動匹配產品的ASIN、UPC或其他資料元素，則必須同時在以下兩處更新資料：您的 [!DNL Commerce] 目錄和 [!DNL Amazon Seller Central] 帳戶。

## 建立Amazon ASIN產品屬性

1. 登入您的 [!DNL Commerce] 管理員。

1. 按一下 **[!UICONTROL Stores]** 的上界。

1. 在 _[!UICONTROL Attributes]_，按一下&#x200B;**[!UICONTROL Product]**.

1. 若要開啟屬性，請按一下 **[!UICONTROL Add New Attribute]**.

1. 針對 **[!UICONTROL Default Label]**，輸入 `Amazon ASIN` （屬性名稱）。

1. 針對 **[!UICONTROL Catalog Input Type for Store Owner]**，選擇 `Text Field`.

1. 針對 **[!UICONTROL Values Required]**，選擇 `No`.

   雖然在Amazon上列出產品需要Amazon ASIN，但您的某些目錄產品可能不會列在Amazon上。

1. 展開 _[!UICONTROL Advanced Attribute Properties]_區段並設定選項：

   - 針對 **[!UICONTROL Attribute Code]**，輸入 `amazon_asin`.

   - 針對 **[!UICONTROL Scope]**，選擇 `Global`.

   - 針對 **[!UICONTROL Unique Value]**，選擇 `No`.

   - 針對 **[!UICONTROL Input Validation for Store Owner]**，選擇 `None`.

   - 針對 **[!UICONTROL Add to Column Options]**，選擇 `Yes`.

   - 針對 **[!UICONTROL Use in Filter Options]**，選擇 `Yes`.

1. 按一下 **[!UICONTROL Save Attribute]**.

![Amazon ASIN屬性](assets/creating-asin-attribute.png)

## 建立Amazon條件產品屬性

1. 登入您的 [!DNL Commerce] 管理員。

1. 按一下 **[!UICONTROL Stores]** 的上界。

1. 在 _[!UICONTROL Attributes]_，按一下&#x200B;**[!UICONTROL Product]**.

1. 要開啟屬性屬性，請按一下 **[!UICONTROL Add New Attribute]**.

1. 針對 **[!UICONTROL Default Label]**，輸入 `Amazon Condition` （屬性名稱）。

1. 針對 **[!UICONTROL Catalog Input Type for Store Owner]**，選擇 `Dropdown`.

   此 _[!UICONTROL Manage Options (Values of your Attribute)]_的上界。

1. 針對 **[!UICONTROL Values Required]**，選擇 `No`.

1. 針對 **[!UICONTROL Manage Options (Values for your Attribute)]**，新增每個條件選項。

   標準Amazon條件包括：

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. 按一下 **[!UICONTROL Add Option]**.

1. 選取 **[!UICONTROL Is Default]** 選項，以取得預設選取範圍。

1. 在 _[!UICONTROL Admin]_欄，輸入要新增條件之標籤的文字(例如 `New`, `Used`，和 `Used-Like New`)

1. 按一下 **[!UICONTROL Add Option]** 視需要新增更多選項。

1. 展開 _[!UICONTROL Advanced Attribute Properties]_，並設定選項。

   - 針對 **[!UICONTROL Attribute Code]**，輸入 `amazon_condition`.

   - 針對 **[!UICONTROL Scope]**，選擇 `Global`.

   - 針對 **[!UICONTROL Unique Value]**，選擇 `No`.

   - 針對 **[!UICONTROL Input Validation for Store Owner]**，選擇 `None`.

   - 針對 **[!UICONTROL Add to Column Options]**，選擇 `Yes`.

   - 針對 **[!UICONTROL Use in Filter Options]**，選擇 `Yes`.

1. 按一下 **[!UICONTROL Save Attribute]**.

![Amazon條件屬性](assets/creating-amazon-condition-attribute.png)

![下一個表徵圖](assets/btn-next.png) [**繼續新增或驗證API金鑰**](./amazon-verify-api-key.md)
