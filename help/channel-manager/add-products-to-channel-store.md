---
title: 新增產品至管道管理員
description: '將目錄中的產品新增至在Channel Manager中設定的銷售管道，以建立 [!DNL Walmart Marketplace] 銷售的產品分類。'
feature: Sales Channels, Merchandising, Products
exl-id: 00932df7-bdc7-42a1-b269-88dffcc918bc
source-git-commit: 0087d60791cf00e4ed2bffe992447ee8e592fd9b
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# 將產品新增至[!DNL Channel Manager]

若要將產品新增至[!DNL Walmart Marketplace]銷售管道，請從[!DNL Commerce]產品目錄中選取產品，並將其匯入至[!DNL Channel Manager]。
視您選取的產品數量而定，匯入程式最多可能需要30分鐘或更長時間。

## 先決條件

**[對應目錄屬性](map-catalog-attributes.md)** — 在[!DNL Channel Settings]組態中，從[!DNL Commerce]產品目錄至少對應一個屬性至其中一個必要的Walmart產品識別碼 —GTIN、ISBN、ISSN、UPC、EAN。

## 清單需求

[!DNL Commerce]產品清單必須具備下列必要的屬性組態：

- **[!UICONTROL Connect to Channel Manager]**&#x200B;屬性已啟用

- 為必要的Walmart屬性提供有效值。

   - 至少有一個產品屬性符合必要的[!DNL Walmart Marketplace]產品識別碼 — GTIN、ISBN、ISSN、UPC、EAN。

   - 產品價格指定至最多兩位小數，例如`9.99`

   - 產品權重指定至最多兩位小數，例如`1.25`

>[!TIP]
>
>如需最佳化銷售管道清單的其他資訊，請參閱[Walmart Marketplace清單品質最佳化指南](https://marketplace.walmart.com/wp-content/uploads/2020/09/WMP_listing_quality_optimization_guide.pdf)。

## 新增產品

1. 從連線的銷售管道存放區中，選取&#x200B;**新增產品**&#x200B;以開啟產品目錄。

   ![新增產品至銷售管道商店](assets/add-initial-products-to-connected-channel.png){width="600" zoomable="yes"}

   目錄會在新標籤中開啟。

1. 從目錄產品格線中，選取要在[!DNL Walmart Marketplace]上銷售的產品。

   ![傳送產品到銷售管道商店](assets/select-products-from-catalog.png){width="600" zoomable="yes"}

1. 啟用所選專案的&#x200B;**[!UICONTROL Connect to Channel Manager]**&#x200B;屬性。

   - 從&#x200B;**[!UICONTROL Actions]**&#x200B;中，選取&#x200B;**[!UICONTROL Update attributes]**。

   - 捲動至&#x200B;**[!UICONTROL Connect to Channel Manager]**&#x200B;屬性並加以啟用。

   - 確認產品屬性至少包含其中一個必要的[!DNL Walmart Product IDs]。

   - 選取&#x200B;**[!UICONTROL Save]**。

     確認訊息隨即顯示。

     ![產品從目錄匯入至銷售管道確認訊息](assets/product-import-from-catalog-confirmation.png){width="400"}

     如果訊息指出更新已排程，請使用[`queue:consumers:start`](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/start-message-queues.html) [!DNL CLI]命令立即處理更新。

     ```bash
     $ bin/magento queue:consumers:start product_action_attribute.update
     ```

1. 匯入作業完成後，請返回[!DNL Channel Manager]並選取&#x200B;**[!UICONTROL Listings]**，以驗證您新增的產品。

   產品一開始處於&#x200B;*草稿*&#x200B;狀態。 選取&#x200B;**[!UICONTROL Refresh products]**&#x200B;以更新資料表。

1. 選取&#x200B;**[!UICONTROL Draft]**&#x200B;狀態卡，更新檢視以顯示新增至管道管理員的新產品。

   ![產品已匯入連線的銷售管道](assets/products-in-marketplace-sales-channel.png){width="400" zoomable="yes"}


