---
title: 屬性
description: AmazonSales Channel提供 [!UICONTROL Attributes] 標籤來監視Amazon和商務屬性清單，以及它們如何對應以進行產品比對。
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 屬性

此 _[!UICONTROL Attributes]_檢視顯示您的Amazon清單， [!DNL Commerce] 屬性。 此清單也會指出已對應以進行產品比對的屬性。 如需詳細資訊，請參閱 [管理屬性](./managing-attributes.md).

![屬性檢視](assets/amazon-attributes-view.png)

從 _[!UICONTROL Attributes]_檢視，並檢閱表格中的屬性設定，以及 [建立或編輯](./creating-attributes.md) 屬性。

## 檢視屬性清單

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**.

1. 按一下 **[!UICONTROL Attributes]** 在左側功能表中，找出Amazon屬性，並檢閱屬性清單。

1. 視需要建立或編輯屬性：

   - 結束日期 [建立](./creating-attributes.md#create-an-attribute) 並定義屬性的匹配屬性值，按一下 **[!UICONTROL Create]**.

   - 停用或 [編輯設定](./creating-attributes.md#edit-an-attribute) 或匹配屬性值，按一下 **[!UICONTROL Edit]**.

      編輯屬性包括為產品匹配更改屬性映射。

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Country] | 中定義的銷售活動的國家/地區  **[!DNL Amazon Marketplace]國家/地區** 期間 [商店整合](./store-integration.md). |
| [!UICONTROL ID] | 由生成的一般屬性值 [!DNL Commerce] 屬性建立時。 |
| [!UICONTROL Amazon Attribute Name] | 從Amazon匯入的屬性名稱。 |
| [!UICONTROL Product Catalog Attribute Code] | 若已對應，則 [!DNL Commerce] 指派給的屬性 _[!UICONTROL Amazon Attribute Name]_以匹配目錄和列出產品。 |
| [!UICONTROL Overwrite Magento Values] | 如果屬性設為 `Overwrite Existing Magento Values` 在「屬性設定」中，表格顯示 `Enabled`. 啟用表示當從Amazon收到屬性的更新產品資訊時，新資訊會更新（覆寫）您 [!DNL Commerce] 目錄。 它也會影響列在 [!DNL Commerce] 商店。 |
| 狀態 | 指出屬性值是否已匯入 [!DNL Commerce] 並對應至 [!DNL Commerce] 屬性。 選項： `Enabled` / `Disabled` |
| 動作 | 指示屬性可用的任務選項。 選項： `Create` / `Edit` |
