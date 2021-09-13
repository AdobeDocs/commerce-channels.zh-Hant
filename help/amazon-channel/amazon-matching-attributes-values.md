---
title: 檢視Amazon屬性對應
description: 驗證連結商務屬性的值，以便在商務和Amazon之間正確同步。
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 檢視Amazon屬性對應

當您將Amazon屬性對應至[!DNL Commerce]屬性時，Amazon銷售管道會追蹤並提供所有Amazon值的可篩選清單。 使用此頁可以驗證連結的[!DNL Commerce]屬性的值在[!DNL Commerce]和Amazon之間正確同步。 您可以檢閱連結或未連結至[!DNL Commerce]屬性之Amazon屬性的同步值。 若要建立或編輯Amazon屬性，請參閱[建立和編輯屬性](./creating-attributes.md)。

_Amazon值_&#x200B;會因您檢視的屬性類型和Amazon屬性而異。 例如，`Label`的列出Amazon值會是文字值，而`AmazonListPrice`則會是數值。 狀態會指出是否已匯入Amazon值。

## 檢視屬性值

1. 在&#x200B;_[!UICONTROL Admin]_側欄上，前往&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找出Amazon屬性，然後按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Create]**或&#x200B;**[!UICONTROL Edit]**。

1. 按一下&#x200B;**[!UICONTROL Matching Attribute Values]**&#x200B;標籤。

   具有相應[!DNL Commerce]目錄產品的清單在&#x200B;_Magento產品SKU_&#x200B;欄中顯示連結值。 按一下連結會開啟對應的目錄產品詳細資料頁面。 產品詳細資料頁面上的Amazon屬性變更不會同步回Amazon銷售管道。

>[!TIP]
>要編輯或分配清單的映射至目錄產品，請參閱[更新必需資訊](./amazon-manually-update-incomplete-listing.md)。

![查看屬性值](assets/amazon-managing-attribute-values.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Region] | 在商店整合期間，在&#x200B;**[!DNL Amazon Marketplace]國家/地區**&#x200B;中定義的銷售活動的地區。 |
| [!UICONTROL Magento Product SKU] | 指出與Amazon商店同步的[!DNL Commerce]產品。 值是[!DNL Commerce]指派的產品ID，並連結至目錄中的產品。 若要在[!DNL Commerce]中開啟產品，請按一下連結。 |
| [!UICONTROL ASIN] | 指示由Amazon為產品標識分配給產品的Amazon標準標識號(ASIN)10個字元的英數字元唯一標識符。 |
| [!UICONTROL Amazon Value] | 指示所選屬性的值。 Amazon值會因您檢視的屬性類型和Amazon屬性而異。 例如，`Label`的列出Amazon值會是文字值，而`AmazonListPrice`則會是數值。 狀態會指出是否已匯入Amazon值。 |
| [!UICONTROL Status] | 指示屬性值是否已導入[!DNL Commerce]並連結到[!DNL Commerce]屬性。 選項：`Not Imported` / `Imported` |
