---
title: 庫存和價格更新
description: '"[!DNL Channel Manager] 同步庫存和價格更新 [!DNL Commerce] 儲存 [!DNL Walmart Marketplace] 以便您可以從 [!DNL Commerce] 管理員'''
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# 更新庫存和定價

[!DNL Channel Manager] 跟蹤產品的庫存和定價 [!DNL Commerce] 產品目錄並同步到連接的銷售渠道的更新， [!DNL Walmart Marketplace]。 同步操作確保產品清單反映當前庫存數量和定價。


>[!IMPORTANT]
>
>之後 [!DNL Channel Manager] 已安裝並配置，所有庫存、價格和訂單更新都將自動同步。 如果已在Walmart Marketplace上銷售，請確保禁用更新產品和訂單資料的任何其他整合。 然後，驗證 [!DNL Commerce] 儲存精確，且與中的資料匹配 [!DNL Walmart Marketplace] 在連接之前 [!DNL Channel Manager] 去現場集市商店。


## 庫存更新

當產品庫存水準在 [!DNL Commerce]。 [!DNL Channel Manager] 同步更新到 [!DNL Walmart Marketplace]。 庫存更新可能需要10分鐘才能跨銷售渠道同步到 [!DNL Walmart marketplace]。

* **更新產品目錄中的庫存數量** — 當 [!DNL Commerce] 庫存數量因 [手動庫存數量更改](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html)退款或取消， [!DNL Channel Manager] 將更改同步到連接的通道， [!DNL Walmart Marketplace]。

* **減少庫存數量以反映 [!DNL Walmart Marketplace] 訂單** — 在 [!DNL Walmart Marketplace] 順序同步到 [!DNL Channel Manager]。 [!DNL Channel Manager] 將更新發送到 [!DNL Commerce] 訂單制度。 [!DNL Commerce] 根據訂單調整庫存數量。 然後，更新的數量將同步到 [!DNL Walmart Marketplace]。 在同步操作完成之前，您可能會在銷售渠道清單和 [!DNL Walmart]。

>[!IMPORTANT]
>
>在 [!DNL Walmart Marketplace] 順序同步到 [!DNL Channel Manager]，庫存數量和訂單資訊僅更新為從 [!DNL Commerce]。 如訂單退還或取消， [!DNL Walmart marketplace]，處理 [!DNL Commerce] 以確保 [!DNL Commerce] 庫存數量和訂單資訊。

## 價格更新

當產品價格在 [!DNL Commerce]。 [!DNL Channel Manager] 將更新同步到 [!DNL Walmart Marketplace]。 最多需要5分鐘，價格更改才能顯示在 [!DNL Walmart Marketplace] 清單。

### 管理連接產品的定價

1. 從 [!UICONTROL Admin]選中 **[!UICONTROL Catalog > Products]**。
1. 在產品網格中，查找要更新的產品並選擇 **[!UICONTROL Edit]**。
1. 根據需要查看和更新價格。
1. **[!UICONTROL Save]** 改變。

有關管理產品價格配置的幫助，請參閱 [!DNL Commerce]，請參閱 [管理定價](https://docs.magento.com/user-guide/catalog/pricing.html){target="_blank"}。
