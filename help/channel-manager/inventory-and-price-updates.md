---
title: 庫存和價格更新
description: '"[!DNL Channel Manager] 同步Commerce商店和 [!DNL Walmart Marketplace] 以便您能夠從Commerce Admin管理您的銷售渠道操作"'
source-git-commit: 2a9bd2f8f91e672786c36f5e132f99bcab59dd00
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 庫存和價格更新

Channel Manager跟蹤已發佈產品的庫存和定價，並同步對Channel Manager和Walmart Marketplace的更改，以反映產品清單中當前庫存數量和定價。**

## 庫存更新

當庫存水準發生變化時，渠道經理會在商務產品目錄和沃爾瑪市場之間同步更新，以便渠道經理和沃爾瑪市場都顯示當前庫存數量。

在渠道經理和沃爾瑪市場中顯示庫存更改可能需要5分鐘。

* **更新產品目錄中的庫存數量** — 如果Commerce庫存數量因 [手動庫存數量更改](https://docs.magento.com/user-guide/catalog/inventory-product-quantity.html) 或訂單退款或取消，渠道經理將更改同步到連接的銷售渠道和 [!DNL Walmart Marketplace]。

* **減少庫存數量以反映沃爾瑪市場訂單** — 在Walmart Marketplace訂單與Channel Manager同步後，Channel Manager將更新發送到Commerce訂單系統。 Commerce根據訂單調整庫存數量。 然後，更新的數量將同步到Walmart Marketplace。 可能是在同步操作完成之前，Channel Manager和Marketplace中顯示的庫存量差異。

>[!IMPORTANT]
>
> 在Walmart Marketplace訂單與渠道經理同步後，庫存數量和其他訂單處理資訊將僅更新為從Commerce啟動的退款和取消。 如果從沃爾瑪市場退還或取消訂單，請處理來自Commerce的更改，以確保Commerce庫存數量和訂單資訊準確。

## 價格更新

當Commerce中的產品價格發生變化時，Channel Manager會將更新從Commerce產品目錄同步到Walmart Marketplace。 顯示清單更改可能需要5分鐘。

### 管理已發佈產品的定價

1. 從 [!UICONTROL Admin]選中 **[!UICONTROL Catalog > Products]**。
1. 在產品網格中，查找要更新的產品並選擇 **[!UICONTROL Edit]**。
1. 根據需要查看和更新價格。
1. **[!UICONTROL Save]** 改變。

Channel Manager將任何價格更新同步到渠道商店和 [!DNL Walmart Marketplace]。 此操作最多需要5分鐘。

有關在Commerce中管理產品價格配置的詳細資訊，請參閱 [管理定價](https://docs.magento.com/user-guide/catalog/pricing.html){target=&quot;_blank&quot;}。
