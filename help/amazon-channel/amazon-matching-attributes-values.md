---
title: 查看Amazon屬性映射
description: 驗證連結的Commerce屬性的值，以在Commerce和Amazon之間正確同步。
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 查看Amazon屬性映射

將Amazon屬性映射到 [!DNL Commerce] 屬性，Amazon銷售渠道跟蹤並提供所有Amazon值的可篩選清單。 使用此頁驗證連結的值 [!DNL Commerce] 屬性在 [!DNL Commerce] 和Amazon。 您可以查看連結或未連結到的Amazon屬性的同步值 [!DNL Commerce] 屬性。 要建立或編輯您的Amazon屬性，請參閱 [建立和編輯屬性](./creating-attributes.md)。

的 _Amazon價值_ 取決於您查看的屬性類型和Amazon屬性。 例如，列出的Amazon值 `Label` 是文本值，而 `AmazonListPrice` 會是個數字。 狀態指示是否已導入Amazon值。

## 查看屬性值

1. 在 _[!UICONTROL Admin]_邊欄，轉到&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

1. 按一下 **[!UICONTROL Attributes]** 在左側菜單中，找到一個Amazon屬性，然後按一下 **[!UICONTROL Create]** 或 **[!UICONTROL Edit]** 的 _[!UICONTROL Action]_的雙曲餘切值。

1. 按一下 **[!UICONTROL Matching Attribute Values]** 頁籤。

   具有相應 [!DNL Commerce] 目錄產品顯示連結的值 _Magento產品SKU_ 的雙曲餘切值。 按一下連結可開啟相應的目錄產品詳細資訊頁面。 對產品詳細資訊頁面上Amazon屬性的更改不會同步回Amazon銷售渠道。

>[!TIP]
>要編輯或分配目錄產品清單的映射，請參閱 [更新所需資訊](./amazon-manually-update-incomplete-listing.md)。

![查看屬性值](assets/amazon-managing-attribute-values.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Region] | 中定義的銷售活動區域 **[!DNL Amazon Marketplace]國家/地區** 在儲存整合期間。 |
| [!UICONTROL Magento Product SKU] | 指示 [!DNL Commerce] 與Amazon店同步的產品。 該值是由 [!DNL Commerce] 連結到目錄中的產品。 在中開啟產品 [!DNL Commerce]，按一下連結。 |
| [!UICONTROL ASIN] | 指示Amazon標準標識號(ASIN)10個字元的字母數字唯一標識符，由Amazon分配給產品以進行產品標識。 |
| [!UICONTROL Amazon Value] | 指示所選屬性的值。 Amazon值因您查看的屬性類型和Amazon屬性而異。 例如，列出的Amazon值 `Label` 是文本值，而 `AmazonListPrice` 會是個數字。 狀態指示是否已導入Amazon值。 |
| [!UICONTROL Status] | 指示屬性值是否已導入 [!DNL Commerce] 和 [!DNL Commerce] 屬性。 選項： `Not Imported` / `Imported` |
