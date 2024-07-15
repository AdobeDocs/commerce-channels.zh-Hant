---
title: 存貨與價格更新
description: '''[!DNL Channel Manager]在 [!DNL Commerce] 商店和 [!DNL Walmart Marketplace] 之間同步庫存和價格更新，以便您可以從 [!DNL Commerce] Admin''管理您的銷售管道作業'
feature: Sales Channels, Merchandising, Inventory, Tools and External Services
role: Leader, Admin, User
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# 更新存貨與定價

[!DNL Channel Manager]追蹤[!DNL Commerce]產品目錄中的產品詳細目錄和定價，並將更新同步至連線的銷售管道和[!DNL Walmart Marketplace]。 同步作業可確保產品清單反映目前的存貨數量與定價。


>[!IMPORTANT]
>
>在安裝及設定[!DNL Channel Manager]之後，所有存貨、價格及訂單更新都會自動同步化。 如果您已在Walmart Marketplace上銷售，請務必停用任何其他可更新產品與訂單資料的整合。 然後，在將[!DNL Channel Manager]連線到即時市集商店之前，請確認[!DNL Commerce]店面中的存貨庫存水準和價格正確無誤，並符合[!DNL Walmart Marketplace]中的資料。


## 詳細目錄更新

當[!DNL Commerce]中的產品詳細目錄等級變更時，[!DNL Channel Manager]會將更新同步至[!DNL Walmart Marketplace]。 若要在銷售管道中將庫存更新同步到[!DNL Walmart marketplace]，最多可能需要10分鐘。

* **產品目錄中的存貨數量更新** — 當[!DNL Commerce]存貨數量因為[手動存貨數量變更](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html)、退款或取消而變更時，[!DNL Channel Manager]會同步處理連線管道和[!DNL Walmart Marketplace]的變更。

* **減少庫存數量以反映[!DNL Walmart Marketplace]個訂單** — 在[!DNL Walmart Marketplace]個訂單同步到[!DNL Channel Manager]之後，[!DNL Channel Manager]會將更新傳送到[!DNL Commerce]個訂單系統。 [!DNL Commerce]會根據順序調整存貨數量。 然後，更新的數量會同步至[!DNL Walmart Marketplace]。 在同步作業完成之前，您可能會在銷售管道清單和[!DNL Walmart]中看到不同的數量。

>[!IMPORTANT]
>
>將[!DNL Walmart Marketplace]訂單同步處理至[!DNL Channel Manager]後，只會針對從[!DNL Commerce]啟動的退款與取消更新存貨數量與訂單資訊。 如果從[!DNL Walmart marketplace]退款或取消訂單，請處理[!DNL Commerce]的變更，以確保[!DNL Commerce]存貨數量與訂單資訊的正確性。

## 價格更新

當[!DNL Commerce]中的產品價格變更時，[!DNL Channel Manager]會將更新同步到[!DNL Walmart Marketplace]。 價格變更最多可能需要5分鐘的時間才會顯示在[!DNL Walmart Marketplace]清單中。

### 管理連線產品的定價

1. 從[!UICONTROL Admin]中，選取&#x200B;**[!UICONTROL Catalog > Products]**。
1. 在產品格線中，尋找要更新的產品並選取&#x200B;**[!UICONTROL Edit]**。
1. 視需要複查並更新價格。
1. **[!UICONTROL Save]**&#x200B;變更。

如需[!DNL Commerce]中管理產品價格設定的協助，請參閱[管理價格](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html)。
