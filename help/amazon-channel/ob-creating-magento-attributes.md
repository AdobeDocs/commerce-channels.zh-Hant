---
title: 建立 [!DNL Commerce] Amazon的屬性
description: 完成Amazon銷售管道入門程式之前，請確定您有所需的[!UICONTROL Commerce]產品屬性。
exl-id: eebad794-c171-40a3-aa24-d5509e2b5797
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# 建立Amazon的[!DNL Commerce]屬性

在上線[!DNL Amazon Seller Central]帳戶之前，最佳作法是新增[!DNL Commerce] [產品屬性](https://docs.magento.com/user-guide/stores/attributes-product.html){:target=&quot;_blank&quot;}以對應您的產品清單。 完成上線後，您可以透過[Amazon銷售管道首頁](./amazon-sales-channel-home.md)頁面的[屬性](./managing-attributes.md)標籤管理產品屬性。

這些指示詳細說明如何為Amazon ASIN和Amazon條件建立[!DNL Commerce]屬性。 建議建立其他屬性，包括Amazon EAN、Amazon ISBN和Amazon UPC。 如果您想要使用Amazon上市價格作為定價規則的價格來源，也可以建立Amazon價格屬性。 在上線期間設定清單和定價設定時，會使用這些屬性。 在建立Amazon清單，以及更新[!DNL Commerce]目錄與您的Amazon清單同步時，也使用這些屬性。

「目錄搜尋」設定可讓您設定相符的搜尋參數，以協助將符合條件的[!DNL Commerce]產品與Amazon清單對應。 映射後，Amazon將激活與定價、數量、改寫、訂單和產品同步相關的操作。

定義這些值會增加完全相符的可能性，將日後手動比對產品清單的需求降至最低。 將屬性新增為上線[預先設定工作](./amazon-pre-setup-tasks.md)的一部分，Amazon銷售管道在上線期間更有可能自動比對產品，並在上線後於Amazon和[!DNL Commerce]之間同步產品資料。

如果您僅建立Amazon ASIN屬性（未為每個產品新增ASIN值），您的[!DNL Commerce]產品可能不會自動符合您的Amazon清單。 您可以透過&#x200B;_Store Review_&#x200B;手動比對產品。 不過，手動比對不會建立共用及同步產品資料所需的資料元素。

>[!IMPORTANT]
>
>如果您更新了手動匹配產品的ASIN、UPC或其他資料元素，則必須同時在以下兩處更新資料：[!DNL Commerce]目錄和[!DNL Amazon Seller Central]帳戶中的清單。

## 建立Amazon ASIN產品屬性

1. 登入您的[!DNL Commerce]管理員。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Stores]**。

1. 在&#x200B;_[!UICONTROL Attributes]_區段中，按一下&#x200B;**[!UICONTROL Product]**。

1. 要開啟屬性屬性，請按一下&#x200B;**[!UICONTROL Add New Attribute]**。

1. 對於&#x200B;**[!UICONTROL Default Label]**，輸入`Amazon ASIN`（屬性的名稱）。

1. 對於&#x200B;**[!UICONTROL Catalog Input Type for Store Owner]**，選擇`Text Field`。

1. 對於&#x200B;**[!UICONTROL Values Required]**，選擇`No`。

   雖然在Amazon上列出產品需要Amazon ASIN，但您的某些目錄產品可能不會列在Amazon上。

1. 展開&#x200B;_[!UICONTROL Advanced Attribute Properties]_區段並設定選項：

   - 對於&#x200B;**[!UICONTROL Attribute Code]**，輸入`amazon_asin`。

   - 對於&#x200B;**[!UICONTROL Scope]**，選擇`Global`。

   - 對於&#x200B;**[!UICONTROL Unique Value]**，選擇`No`。

   - 對於&#x200B;**[!UICONTROL Input Validation for Store Owner]**，選擇`None`。

   - 對於&#x200B;**[!UICONTROL Add to Column Options]**，選擇`Yes`。

   - 對於&#x200B;**[!UICONTROL Use in Filter Options]**，選擇`Yes`。

1. 按一下&#x200B;**[!UICONTROL Save Attribute]**。

![Amazon ASIN屬性](assets/creating-asin-attribute.png)

## 建立Amazon條件產品屬性

1. 登入您的[!DNL Commerce]管理員。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Stores]**。

1. 在&#x200B;_[!UICONTROL Attributes]_區段中，按一下&#x200B;**[!UICONTROL Product]**。

1. 要開啟屬性屬性，請按一下&#x200B;**[!UICONTROL Add New Attribute]**。

1. 對於&#x200B;**[!UICONTROL Default Label]**，輸入`Amazon Condition`（屬性的名稱）。

1. 對於&#x200B;**[!UICONTROL Catalog Input Type for Store Owner]**，選擇`Dropdown`。

   將顯示&#x200B;_[!UICONTROL Manage Options (Values of your Attribute)]_部分。

1. 對於&#x200B;**[!UICONTROL Values Required]**，選擇`No`。

1. 對於&#x200B;**[!UICONTROL Manage Options (Values for your Attribute)]**，新增每個條件選項。

   標準Amazon條件包括：

   - `New: Refurbished: Used`
   - `Like New: Used`
   - `Very Good: Used`
   - `Good: Used`
   - `Acceptable: Collectible`
   - `Like New; Collectible`
   - `Very Good: Collectible`
   - `Good: Collectible; Acceptable`

1. 按一下&#x200B;**[!UICONTROL Add Option]**。

1. 為您希望成為預設選擇的條件選擇&#x200B;**[!UICONTROL Is Default]**&#x200B;選項。

1. 在&#x200B;_[!UICONTROL Admin]_欄中，輸入要添加條件的標籤文本（如`New`、`Used`和`Used-Like New`）

1. 視需要按一下&#x200B;**[!UICONTROL Add Option]**&#x200B;以新增更多選項。

1. 展開&#x200B;_[!UICONTROL Advanced Attribute Properties]_區段並設定選項。

   - 對於&#x200B;**[!UICONTROL Attribute Code]**，輸入`amazon_condition`。

   - 對於&#x200B;**[!UICONTROL Scope]**，選擇`Global`。

   - 對於&#x200B;**[!UICONTROL Unique Value]**，選擇`No`。

   - 對於&#x200B;**[!UICONTROL Input Validation for Store Owner]**，選擇`None`。

   - 對於&#x200B;**[!UICONTROL Add to Column Options]**，選擇`Yes`。

   - 對於&#x200B;**[!UICONTROL Use in Filter Options]**，選擇`Yes`。

1. 按一下&#x200B;**[!UICONTROL Save Attribute]**。

![Amazon條件屬性](assets/creating-amazon-condition-attribute.png)

![下一](assets/btn-next.png) [**個圖示繼續新增或驗證API金鑰**](./amazon-verify-api-key.md)
