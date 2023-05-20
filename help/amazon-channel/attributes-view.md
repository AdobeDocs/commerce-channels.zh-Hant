---
title: 屬性
description: AmazonSales Channel提供 [!UICONTROL Attributes] 頁籤，以監視Amazon和Commerce屬性的清單以及它們如何映射以進行產品匹配。
exl-id: fc08cd6e-eef9-4e71-82b1-5443e14800ce
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# 屬性

的 _[!UICONTROL Attributes]_視圖顯示您的Amazon和 [!DNL Commerce] 屬性。 該清單還指示已映射用於產品匹配的屬性。 有關詳細資訊，請參見 [管理屬性](./managing-attributes.md)。

![屬性視圖](assets/amazon-attributes-view.png)

從 _[!UICONTROL Attributes]_查看，並查看表和 [建立或編輯](./creating-attributes.md) 屬性。

## 查看屬性清單

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Marketing]** > _[!UICONTROL Channels]_>**[!UICONTROL Amazon Sales Channel]**。

1. 按一下 **[!UICONTROL Attributes]** 在左側菜單中，找到一個Amazon屬性，然後查看屬性清單。

1. 根據需要建立或編輯屬性：

   - 至 [建立](./creating-attributes.md#create-an-attribute) 並為屬性定義匹配屬性值，按一下 **[!UICONTROL Create]**。

   - 停用或 [編輯設定](./creating-attributes.md#edit-an-attribute) 或匹配屬性的屬性值，按一下 **[!UICONTROL Edit]**。

      編輯屬性包括更改產品匹配的屬性映射。

| 欄位 | 說明 |
|--- |--- |
| [!UICONTROL Country] | 在中定義的銷售活動的國家/地區  **[!DNL Amazon Marketplace]國家/地區** 在 [儲存整合](./store-integration.md)。 |
| [!UICONTROL ID] | 生成的泛型屬性值 [!DNL Commerce] 建立屬性時。 |
| [!UICONTROL Amazon Attribute Name] | 從Amazon導入的屬性的名稱。 |
| [!UICONTROL Product Catalog Attribute Code] | 如果映射， [!DNL Commerce] 分配給映射到的屬性 _[!UICONTROL Amazon Attribute Name]_用於匹配目錄和列出產品。 |
| [!UICONTROL Overwrite Magento Values] | 如果屬性設定為 `Overwrite Existing Magento Values` 在「屬性設定」(Attribute Settings)中，該表顯示 `Enabled`。 啟用表示當從Amazon接收到屬性的更新產品資訊時，新資訊將更新（覆蓋）您的 [!DNL Commerce] 目錄。 它還會影響您在 [!DNL Commerce] 商店。 |
| 狀態 | 指示屬性值是否已導入 [!DNL Commerce] 映射到 [!DNL Commerce] 屬性。 選項： `Enabled` / `Disabled` |
| 操作 | 指示屬性可用的任務選項。 選項： `Create` / `Edit` |
