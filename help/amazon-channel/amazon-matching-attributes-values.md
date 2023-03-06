---
title: 檢視Amazon屬性對應
description: 驗證連結商務屬性的值，以便在商務和Amazon之間正確同步。
exl-id: 11a1fb25-6aa8-43d3-b5d8-772bbe1a5d53
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 檢視Amazon屬性對應

將Amazon屬性對應至 [!DNL Commerce] 屬性，Amazon銷售管道會追蹤並提供所有Amazon值的可篩選清單。 使用此頁可驗證連結的值 [!DNL Commerce] 屬性之間正確同步 [!DNL Commerce] 和Amazon。 您可以檢閱已連結或未連結至的Amazon屬性的同步值 [!DNL Commerce] 屬性。 若要建立或編輯您的Amazon屬性，請參閱 [建立和編輯屬性](./creating-attributes.md).

此 _Amazon值_ 會依您檢視的屬性類型和Amazon屬性而有所不同。 例如，列出的Amazon值 `Label` 會是文字值，而 `AmazonListPrice` 會是數值。 狀態會指出是否已匯入Amazon值。

## 檢視屬性值

1. 在 _[!UICONTROL Admin]_邊欄，轉到&#x200B;**[!UICONTROL Marketing]**>_[!UICONTROL Channels]_ > **[!UICONTROL Amazon Sales Channel]**.

1. 按一下 **[!UICONTROL Attributes]** 在左側功能表中，找出Amazon屬性，然後按一下 **[!UICONTROL Create]** 或 **[!UICONTROL Edit]** 在 _[!UICONTROL Action]_欄。

1. 按一下 **[!UICONTROL Matching Attribute Values]** 標籤。

   具有相應 [!DNL Commerce] 目錄產品在 _Magento產品SKU_ 欄。 按一下連結會開啟對應的目錄產品詳細資料頁面。 產品詳細資料頁面上的Amazon屬性變更不會同步回Amazon銷售管道。

>[!TIP]
>若要編輯或指派清單的對應至目錄產品，請參閱 [更新所需資訊](./amazon-manually-update-incomplete-listing.md).

![查看屬性值](assets/amazon-managing-attribute-values.png)

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Region] | 中定義的銷售活動的地區 **[!DNL Amazon Marketplace]國家/地區** 儲存整合期間。 |
| [!UICONTROL Magento Product SKU] | 指出 [!DNL Commerce] 與Amazon商店同步的產品。 值是指派的產品ID [!DNL Commerce] 連結到目錄中的產品。 若要在中開啟產品 [!DNL Commerce]，按一下連結。 |
| [!UICONTROL ASIN] | 指示由Amazon為產品標識分配給產品的Amazon標準標識號(ASIN)10個字元的英數字元唯一標識符。 |
| [!UICONTROL Amazon Value] | 指示所選屬性的值。 Amazon值會因您檢視的屬性類型和Amazon屬性而異。 例如，列出的Amazon值 `Label` 會是文字值，而 `AmazonListPrice` 會是數值。 狀態會指出是否已匯入Amazon值。 |
| [!UICONTROL Status] | 指出屬性值是否已匯入 [!DNL Commerce] 連結到 [!DNL Commerce] 屬性。 選項： `Not Imported` / `Imported` |
