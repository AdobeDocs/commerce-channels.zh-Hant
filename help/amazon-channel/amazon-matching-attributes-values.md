---
title: 檢視Amazon屬性對應
description: 驗證連結Commerce屬性的值，以在Commerce與Amazon之間正確同步。
feature: Sales Channels, Products, Configuration
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 檢視Amazon屬性對應

當您將Amazon屬性對應至[!DNL Commerce]屬性時，Amazon sales channel會追蹤並提供所有Amazon值的可篩選清單。 使用此頁面來驗證您連結的[!DNL Commerce]屬性的值，以便在[!DNL Commerce]和Amazon之間正確同步。 您可以檢閱連結或未連結至[!DNL Commerce]屬性之Amazon屬性的同步值。 若要建立或編輯您的Amazon屬性，請參閱[建立和編輯屬性](./creating-attributes.md)。

_Amazon值_&#x200B;會依您檢視的屬性型別和Amazon屬性而有所不同。 例如，`Label`的已列出Amazon值會是文字值，而`AmazonListPrice`則是數值量。 狀態會指出Amazon值是否已匯入。

## 檢視您的屬性值

1. 在&#x200B;_[!UICONTROL Admin]_側邊欄上，前往&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找到Amazon屬性，然後按一下&#x200B;_[!UICONTROL Action]_欄中的&#x200B;**[!UICONTROL Create]**或&#x200B;**[!UICONTROL Edit]**。

1. 按一下「**[!UICONTROL Matching Attribute Values]**」標籤。

   具有對應[!DNL Commerce]目錄產品的清單會在&#x200B;_[!UICONTROL Magento Product SKU]_欄中顯示連結的值。 按一下連結會開啟對應的目錄產品詳細資料頁面。 產品詳細資料頁面上Amazon屬性的變更不會同步回Amazon銷售管道。

>[!TIP]
>若要編輯或指派清單對應至目錄產品，請參閱[更新必要資訊](./amazon-manually-update-incomplete-listing.md)。

![檢視屬性值](assets/amazon-managing-attribute-values.png){width="600" zoomable="yes"}

| 欄位 | 說明 |
|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Region] | 商店整合期間在&#x200B;**[!DNL Amazon Marketplace]國家/地區**&#x200B;中定義的銷售活動區域。 |
| [!UICONTROL Magento Product SKU] | 表示與Amazon市集同步的[!DNL Commerce]產品。 此值是由[!DNL Commerce]指派的產品ID，並連結至目錄中的產品。 若要在[!DNL Commerce]中開啟產品，請按一下連結。 |
| [!UICONTROL ASIN] | 表示Amazon針對產品識別指派給產品的Amazon標準識別碼(ASIN) 10個字元英數字元唯一識別碼。 |
| [!UICONTROL Amazon Value] | 指示所選屬性的值。 Amazon值會依您檢視的屬性型別和Amazon屬性而有所不同。 例如，`Label`的已列出Amazon值會是文字值，而`AmazonListPrice`則是數值量。 狀態會指出Amazon值是否已匯入。 |
| [!UICONTROL Status] | 表示屬性值是否已匯入至[!DNL Commerce]並連結至[!DNL Commerce]屬性。 選項： `Not Imported` / `Imported` |
