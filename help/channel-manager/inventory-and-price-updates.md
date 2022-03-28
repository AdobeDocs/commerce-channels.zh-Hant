---
title: 庫存和價格更新
description: '"[!DNL Channel Manager] 同步Commerce商店和 [!DNL Walmart Marketplace] 以便您能夠從Commerce Admin管理您的銷售渠道操作'''
exl-id: 4dd9fa4a-b12f-4795-a7b2-84ea0fc26aa5
source-git-commit: a1944052f02968c36495275cd5ddfb2ca43ce967
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 庫存和價格更新

[!DNL Channel Manager] 跟蹤渠道商店中產品的庫存和定價。 當庫存或定價發生更改時，更新將同步到兩者 [!DNL Channel Manager] 和 [!DNL Walmart Marketplace] 反映產品清單中當前庫存數量和定價。

## 庫存更新

當庫存水準發生變化時，渠道經理會同步Commerce和Walmart Marketplace之間的更新，以確保渠道經理和Walmart Marketplace擁有正確的庫存數量。

在Channel Manager和市場之間同步清單更新可能需要10分鐘。

* **更新產品目錄中的庫存數量** — 當Commerce庫存數量因 [手動庫存數量更改](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html)、退款或取消，Channel Manager將更改同步到連接的渠道和 [!DNL Walmart Marketplace]。

* **減少庫存數量以反映沃爾瑪市場訂單** — 在Walmart Marketplace訂單與Channel Manager同步後，Channel Manager將更新發送到Commerce訂單系統。 Commerce根據訂單調整庫存數量。 然後，更新的數量將同步到Walmart Marketplace。 在同步操作完成之前，您可能會看到Channel Manager和Marketplace之間的數量差異。

>[!IMPORTANT]
>
> 在Walmart Marketplace訂單同步到Channel Manager後，庫存數量和訂單資訊只會更新為從Commerce啟動的退款和取消。 如果從沃爾瑪市場退還或取消訂單，則處理從Commerce進行的更改，以確保Commerce庫存數量和訂單資訊的準確性。

## 價格更新

當Commerce中的產品價格更改時，Channel Manager將從 [!DNL Commerce] 產品目錄 [!DNL Walmart Marketplace]。 市場顯示價格變化可能需要5分鐘。

### 管理已發佈產品的定價

1. 從 [!UICONTROL Admin]選中 **[!UICONTROL Catalog > Products]**。
1. 在產品網格中，查找要更新的產品並選擇 **[!UICONTROL Edit]**。
1. 根據需要查看和更新價格。
1. **[!UICONTROL Save]** 改變。

有關在Commerce中管理產品價格配置的詳細資訊，請參閱 [管理定價](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}。
