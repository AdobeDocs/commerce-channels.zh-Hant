---
title: 將產品添加到銷售渠道商店
description: 建立產品分類 [!DNL Walmart Marketplace] 通過將產品從目錄添加到銷售渠道進行銷售
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: d9b39984fc7401c42fc431f35cf5649f86f4f2f9
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# 將產品添加到 [!DNL Channel Manager]

將產品添加到 [!DNL Walmart Marketplace] 銷售渠道，從 [!DNL Commerce] 將產品目錄導入 [!DNL Channel Manager]。
根據您選擇的產品數量，導入過程可能需要30分鐘或更長時間。

## 先決條件

**[映射目錄屬性](map-catalog-attributes.md)** — 在 [!DNL Channel Settings] 配置，映射至少一個屬性 [!DNL Commerce] 將產品目錄添加到所需的沃爾瑪產品標識符之一 — GTIN、ISBN、ISSN、UPC、EAN。

## 上市要求

[!DNL Commerce] 產品清單必須具有以下必需的屬性配置：

- **[!UICONTROL Connect to Channel Manager]** 屬性已啟用

- 為所需的Walmart屬性提供有效值。

   - 至少一個與所需的 [!DNL Walmart Marketplace] 產品標識符 — GTIN、ISBN、ISSN、UPC、EAN。

   - 指定的產品價格最多為兩個小數位，例如 `9.99`

   - 指定的產品重量最多為兩個小數位，例如 `1.25`

>[!TIP]
>
>有關優化銷售渠道清單的其他資訊，請參閱 [《沃爾瑪市場清單質量優化指南》](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf)。

## 添加產品

1. 從連接的銷售渠道商店中，選擇 **添加產品** 開啟產品目錄。

   ![將產品添加到銷售渠道商店](assets/add-initial-products-to-connected-channel.png)

   目錄將在新頁籤中開啟。

1. 從目錄產品網格中，選擇要銷售的產品 [!DNL Walmart Marketplace]。

   ![將產品發送到銷售渠道商店](assets/select-products-from-catalog.png)

1. 啟用 **[!UICONTROL Connect to Channel Manager]** 屬性。

   - 從 **[!UICONTROL Actions]**&#x200B;選中 **[!UICONTROL Update attributes]**。

   - 滾動到 **[!UICONTROL Connect to Channel Manager]** 屬性並啟用它。

   - 驗證產品屬性是否至少包括所需的 [!DNL Walmart Product IDs]。

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

