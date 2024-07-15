---
title: Amazon清單的屬性
description: AmazonSales Channel提供[!UICONTROL Attributes]標籤以監視Amazon和Commerce屬性清單，以及如何對應它們以進行產品比對。
feature: Sales Channels, Products, Configuration
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Amazon清單的屬性

_[!UICONTROL Attributes]_檢視會顯示您的Amazon和[!DNL Commerce]屬性清單。 此清單也會指出已對應產品比對的屬性。 如需詳細資訊，請參閱[管理屬性](./managing-attributes.md)。

![屬性檢視](assets/amazon-attributes-view.png){width="600" zoomable="yes"}

從&#x200B;_[!UICONTROL Attributes]_檢視中，您和您檢閱資料表中的屬性設定，並[建立或編輯](./creating-attributes.md)屬性。

## 檢視您的屬性清單

1. 在&#x200B;_管理員_&#x200B;側邊欄上，移至&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找到Amazon屬性，然後檢閱您的屬性清單。

1. 視需要建立或編輯屬性：

   - 若要[建立](./creating-attributes.md#create-an-attribute)並定義屬性的相符屬性值，請按一下&#x200B;**[!UICONTROL Create]**。

   - 若要停用或[編輯屬性的設定](./creating-attributes.md#edit-an-attribute)或相符的屬性值，請按一下&#x200B;**[!UICONTROL Edit]**。

     編輯屬性包括變更產品比對的屬性對應。

| 欄位 | 說明 |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Country] | 在[商店整合](./store-integration.md)期間，**[!DNL Amazon Marketplace]國家**&#x200B;中定義的銷售活動國家/地區。 |
| [!UICONTROL ID] | [!DNL Commerce]在建立屬性時產生的泛型屬性值。 |
| [!UICONTROL Amazon Attribute Name] | 從Amazon匯入的屬性名稱。 |
| [!UICONTROL Product Catalog Attribute Code] | 如果已對應，則指派給對應至&#x200B;_[!UICONTROL Amazon Attribute Name]_的[!DNL Commerce]屬性會用於比對目錄和列出產品。 |
| [!UICONTROL Overwrite Magento Values] | 如果屬性設定中的屬性設定為`Overwrite Existing Magento Values`，表格會顯示`Enabled`。 啟用表示從Amazon收到屬性的更新產品資訊時，新資訊會更新（覆寫） [!DNL Commerce]目錄中產品的對應資訊。 它也會影響您的[!DNL Commerce]商店中列出的產品。 |
| 狀態 | 表示屬性值是否已匯入至[!DNL Commerce]並對應至[!DNL Commerce]屬性。 選項： `Enabled` / `Disabled` |
| 動作 | 表示屬性可用的工作選項。 選項： `Create` / `Edit` |
