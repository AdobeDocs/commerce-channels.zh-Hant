---
title: 將產品添加到連接的渠道
description: 通過將產品從目錄添加到銷售渠道為市場銷售建立產品分類
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: e6368d30e16ccffcb1dfc64bdd56561116934b54
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 將產品添加到連接的渠道

要將產品同步到Walmart Marketplace銷售渠道，請從 [!DNL Commerce] 將產品目錄導入Channel Manager。 所選產品必須具有以下屬性配置：

- **[!UICONTROL Publish to Channel Manager]** 屬性已啟用

- 至少有一個產品屬性必須與 [必需的Walmart Marketplace屬性](map-product-attributes-for-matching.md)-GTIN、ISBN、ISSN、UPC、EAN

從導入產品的流程 [!DNL Commerce] 到Channel Manager最多需要30分鐘或更長時間，具體取決於您選擇的產品數。

## 將產品添加到銷售渠道

1. 從連接的銷售渠道商店中，選擇 **添加產品** 開啟產品目錄。

   ![將產品添加到連接的渠道](assets/add-initial-products-to-connected-channel.png)

   目錄將在新頁籤中開啟。

1. 從目錄產品網格中，選擇要銷售的產品 [!DNL Walmart Marketplace]。

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

1. 導入操作完成後，查看產品 **[!UICONTROL Listings]**。

   ![導入到連接銷售渠道的產品](assets/products-in-marketplace-sales-channel.png)

   最初，產品 *草稿* 狀態。 選擇 **[!UICONTROL Refresh products]** 按鈕。

