---
title: 將產品添加到銷售渠道商店
description: 建立產品分類 [!DNL Walmart Marketplace] 通過將產品從目錄添加到銷售渠道進行銷售
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 76aa7451c9df83fbb7ea808fc14ef2d306235da2
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# 將產品添加到銷售渠道商店

要將產品同步到Walmart Marketplace銷售渠道，請從 [!DNL Commerce] 將產品目錄導入Channel Manager。 所選產品必須具有以下屬性配置：

- **[!UICONTROL Publish to Channel Manager]** 屬性已啟用

- 至少有一個產品屬性必須與 [必需的Walmart Marketplace屬性](map-product-attributes-for-matching.md)-GTIN、ISBN、ISSN、UPC、EAN

從導入產品的流程 [!DNL Commerce] 到Channel Manager最多需要30分鐘或更長時間，具體取決於您選擇的產品數。

## 添加產品

1. 從連接的銷售渠道商店中，選擇 **添加產品** 開啟產品目錄。

   ![將產品添加到銷售渠道商店](assets/add-initial-products-to-connected-channel.png)

   目錄將在新頁籤中開啟。

1. 從目錄產品網格中，選擇要銷售的產品 [!DNL Walmart Marketplace]。

   ![將產品發送到銷售渠道商店](assets/select-products-from-catalog.png)

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

1. 導入操作完成後，通過返回到 [!DNL Channel Manager] 選擇 **[!UICONTROL Listings]**。

   ![導入到連接銷售渠道的產品](assets/products-in-marketplace-sales-channel.png)

   最初，產品 *草稿* 狀態。 選擇 **[!UICONTROL Refresh products]** 按鈕。

