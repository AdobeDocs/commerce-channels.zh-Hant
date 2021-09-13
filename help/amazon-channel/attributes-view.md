---
title: 屬性
description: AmazonSales Channel提供[!UICONTROL Attributes]標籤，以監控Amazon和商務屬性清單，以及如何對應這些屬性以進行產品比對。
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 屬性

_[!UICONTROL Attributes]_檢視會顯示您的Amazon和[!DNL Commerce]屬性清單。 此清單也會指出已對應以進行產品比對的屬性。 如需詳細資訊，請參閱[管理屬性](./managing-attributes.md)。

![屬性檢視](assets/amazon-attributes-view.png)

從&#x200B;_[!UICONTROL Attributes]_視圖中，查看表中的屬性設定，並[建立或編輯](./creating-attributes.md)屬性。

## 檢視屬性清單

1. 在&#x200B;_Admin_&#x200B;側欄中，前往&#x200B;**[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下左側功能表中的&#x200B;**[!UICONTROL Attributes]**，找出Amazon屬性，並檢閱屬性清單。

1. 視需要建立或編輯屬性：

   - 要[create](./creating-attributes.md#create-an-attribute)並定義屬性的匹配屬性值，請按一下&#x200B;**[!UICONTROL Create]**。

   - 要停用或編輯屬性的設定](./creating-attributes.md#edit-an-attribute)或匹配屬性值，請按一下&#x200B;**[!UICONTROL Edit]**。[

      編輯屬性包括為產品匹配更改屬性映射。

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Country] | 在[商店整合](./store-integration.md)期間，在&#x200B;**[!DNL Amazon Marketplace]國家/地區**&#x200B;中定義的銷售活動的國家/地區。 |
| [!UICONTROL ID] | 建立屬性時由[!DNL Commerce]產生的一般屬性值。 |
| [!UICONTROL Amazon Attribute Name] | 從Amazon匯入的屬性名稱。 |
| [!UICONTROL Product Catalog Attribute Code] | 如果已映射，則為[!DNL Commerce]分配的屬性將映射到&#x200B;_[!UICONTROL Amazon Attribute Name]_以匹配目錄和列出產品。 |
| [!UICONTROL Overwrite Magento Values] | 如果「屬性設定」中的屬性設為`Overwrite Existing Magento Values`，則表格會顯示`Enabled`。 啟用表示從Amazon收到屬性的更新產品資訊時，新資訊會更新（覆寫）[!DNL Commerce]目錄中產品的對應資訊。 它也會影響[!DNL Commerce]商店中列出的產品。 |
| 狀態 | 指示屬性值是否已導入[!DNL Commerce]並映射到[!DNL Commerce]屬性。 選項：`Enabled` / `Disabled` |
| 動作 | 指示屬性可用的任務選項。 選項：`Create` / `Edit` |
