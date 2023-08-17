---
title: 存貨與價格更新
description: 『[!DNL Channel Manager] 同步處理存貨與價格更新 [!DNL Commerce] 存放區和 [!DNL Walmart Marketplace] 這樣您就可以從以下管理銷售管道作業： [!DNL Commerce] 管理員'
feature: Sales Channels, Merchandising, Inventory, Tools and External Services
role: Leader, Admin, User
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 更新存貨與定價

[!DNL Channel Manager] 追蹤中產品的存貨和定價 [!DNL Commerce] 產品目錄並將更新同步至連線的銷售管道和 [!DNL Walmart Marketplace]. 同步作業可確保產品清單反映目前的存貨數量與定價。


>[!IMPORTANT]
>
>晚於 [!DNL Channel Manager] 已安裝並設定，所有存貨、價格及訂單更新會自動同步。 如果您已在Walmart Marketplace上銷售，請務必停用任何其他可更新產品與訂單資料的整合。 然後，確認存貨量水準與價格在 [!DNL Commerce] 店面準確且符合中的資料 [!DNL Walmart Marketplace] 連線之前 [!DNL Channel Manager] 前往即時市集商店。


## 詳細目錄更新

當產品存貨層次在中變更時 [!DNL Commerce]， [!DNL Channel Manager] 將更新同步至 [!DNL Walmart Marketplace]. 庫存更新最多可能需要10分鐘，才能在銷售管道間同步至 [!DNL Walmart marketplace].

* **產品目錄中的庫存數量更新** — 當 [!DNL Commerce] 庫存數量變更的原因為 [手動庫存數量變更](https://experienceleague.adobe.com/docs/commerce-admin/inventory/quantities/quantities-assign-per-product.html)，退款或取消， [!DNL Channel Manager] 將變更同步至已連線的通道，並 [!DNL Walmart Marketplace].

* **減少庫存量以反映 [!DNL Walmart Marketplace] 訂購** — 在 [!DNL Walmart Marketplace] 訂單同步至 [!DNL Channel Manager]， [!DNL Channel Manager] 傳送更新至 [!DNL Commerce] 訂購系統。 [!DNL Commerce] 會根據順序調整庫存數量。 然後，更新後的數量會同步至 [!DNL Walmart Marketplace]. 在同步作業完成之前，您可能會在sales channel清單和中看到不同的數量 [!DNL Walmart].

>[!IMPORTANT]
>
>之後 [!DNL Walmart Marketplace] 訂單同步至 [!DNL Channel Manager]，存貨數量與訂單資訊僅會針對起始「退款」與「取消」更新 [!DNL Commerce]. 如果訂單已退款或取消自 [!DNL Walmart marketplace]，處理變更，從 [!DNL Commerce] 以確保的正確性 [!DNL Commerce] 存貨數量與訂單資訊。

## 價格更新

當產品價格在 [!DNL Commerce]， [!DNL Channel Manager] 將更新同步至 [!DNL Walmart Marketplace]. 價格變更最多可能需要5分鐘的時間才會顯示在 [!DNL Walmart Marketplace] 清單。

### 管理連線產品的定價

1. 從 [!UICONTROL Admin]，選取 **[!UICONTROL Catalog > Products]**.
1. 在產品格線中，尋找要更新的產品並選取 **[!UICONTROL Edit]**.
1. 視需要複查並更新價格。
1. **[!UICONTROL Save]** 變更。

如需管理產品價格設定的相關協助，請參閱： [!DNL Commerce]，請參閱 [管理定價](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/pricing-advanced.html).
