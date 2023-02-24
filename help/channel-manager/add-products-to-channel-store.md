---
title: 將產品新增至Channel Manager
description: '''建立產品分類 [!DNL Walmart Marketplace] 將產品從目錄新增至渠道管理員中設定的銷售渠道，以實現銷售。 '
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# 將產品新增至 [!DNL Channel Manager]

若要將產品新增至 [!DNL Walmart Marketplace] 銷售渠道，從 [!DNL Commerce] 產品目錄，並匯入 [!DNL Channel Manager].
根據您選取的產品數量，匯入程式最多需要30分鐘或更久。

## 先決條件

**[映射目錄屬性](map-catalog-attributes.md)** — 在 [!DNL Channel Settings] 配置，映射至少一個屬性 [!DNL Commerce] 產品目錄，指向所需的Walmart產品標識符之一 — GTIN、ISBN、ISSN、UPC、EAN。

## 上市要求

[!DNL Commerce] 產品清單必須具備下列必要的屬性設定：

- **[!UICONTROL Connect to Channel Manager]** 屬性已啟用

- 為所需的Walmart屬性提供有效值。

   - 至少有一個產品屬性符合其中一個必要的 [!DNL Walmart Marketplace] 產品標識符 — GTIN、ISBN、ISSN、UPC、EAN。

   - 指定的產品價格最多兩位小數，例如 `9.99`

   - 指定的產品重量最多為兩位小數，例如 `1.25`

>[!TIP]
>
>有關優化銷售渠道清單的其他資訊，請參閱 [Walmart Marketplace上市質量優化指南](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf).

## 新增產品

1. 從連接的銷售渠道商店中，選擇 **新增產品** 以開啟產品目錄。

   ![將產品添加到銷售渠道商店](assets/add-initial-products-to-connected-channel.png)

   目錄會在新索引標籤中開啟。

1. 從目錄產品網格中，選擇要銷售的產品 [!DNL Walmart Marketplace].

   ![將產品傳送至銷售渠道商店](assets/select-products-from-catalog.png)

1. 啟用 **[!UICONTROL Connect to Channel Manager]** 屬性。

   - 從 **[!UICONTROL Actions]**，選取 **[!UICONTROL Update attributes]**.

   - 捲動至 **[!UICONTROL Connect to Channel Manager]** 屬性並加以啟用。

   - 確認產品屬性包含至少一個所需的 [!DNL Walmart Product IDs].

   - 選擇 **[!UICONTROL Save]**.

      隨即顯示確認訊息。

      ![產品從目錄匯入至銷售管道確認訊息](assets/product-import-from-catalog-confirmation.png)

      如果訊息指出已排程更新，請使用 [佇列:consumers:開始](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-queue.html) [!DNL CLI] 命令立即處理更新。

      ```bash
      $ bin/magento queue:consumers:start product_action_attribute.update
      ```

1. 匯入作業完成後，請回到 [!DNL Channel Manager] 選取 **[!UICONTROL Listings]**.

   起初，產品位於 *草稿* 狀態。 選擇 **[!UICONTROL Refresh products]** 以更新表格。

1. 更新檢視以顯示新增至管道管理員的新產品，方法是選取 **[!UICONTROL Draft]** 狀態卡。

   ![導入到連接銷售渠道的產品](assets/products-in-marketplace-sales-channel.png)


