---
title: 將產品添加到渠道商店
description: 通過將產品從目錄添加到銷售渠道為市場銷售建立產品分類
source-git-commit: 905bedaf1eacdc45b2b7f222e7703e1f7b3dfd9c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 將產品添加到渠道商店

從Channel Manager中，從 [!DNL Commerce] 沃爾瑪市場銷售目錄。

要將產品同步到銷售渠道，所選產品必須具有以下屬性配置：

- **[!UICONTROL Publish to Channel Manager]** 屬性已啟用

- 至少有一個產品屬性必須與 [必需的Walmart Marketplace屬性](map-product-attributes-for-matching.md)-GTIN、ISBN、ISSN、UPC、EAN

保存選擇後，Channel Manager會將產品資料導入渠道。 此過程最多需要30分鐘。

## 將產品添加到銷售渠道

1. 開啟與Channel Manager商店關聯的產品目錄。

   從連接的銷售渠道商店中，選擇 **添加產品**。

   ![將產品添加到連接的渠道](assets/add-initial-products-to-connected-channel.png)

   目錄將在新頁籤中開啟。

1. 從目錄產品網格中，選擇要在Walmart Marketplace上銷售的產品。

   ![將產品發送到連接的渠道](assets/select-products-from-catalog.png)

1. 啟用 **[!UICONTROL Publish to Channel Manager]** 屬性。

   - 從 **[!UICONTROL Actions]**&#x200B;選中 **[!UICONTROL Update attributes]**。

   - 滾動到 **[!UICONTROL Publish to Channel Manager]** 屬性並啟用它。

   - 驗證產品屬性是否至少包括所需的沃爾瑪產品ID之一。

   - 選擇 **[!UICONTROL Save]**。

   將顯示確認消息。

   ![產品從目錄導入到銷售渠道確認消息](assets/product-import-from-catalog-confirmation.png)

   如果消息指示已計畫更新，請使用 [隊列:consumers:開始](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] 命令立即處理更新。

   ```bash
   $ bin/magento queue:consumers:start product_action_attribute.update
   ```

1. 返回至中的連接銷售渠道 [!DNL Channel Manager]。

   導入操作完成後，查看產品 **[!UICONTROL Listings]**。 最初，產品 *草稿* 狀態。 選擇 [!UICONTROL Refresh products]**更新表。

   ![導入到連接銷售渠道的產品](assets/products-in-marketplace-sales-channel.png)
