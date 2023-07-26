---
title: Amazon銷售管道 — 價格範圍
description: 使用商務定價範圍，根據多個網站或全域管理定價。
feature: Sales Channels, Price Rules
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# 價格範圍

[!DNL Commerce] 提供設定，用於 [定價範圍](https://experienceleague.adobe.com/docs/commerce-admin/config/catalog/catalog.html#price) 將設為 `Global` 或 `Website`. 如果訂價設為 `Global`，所有網站都有單一價格來源。 如果訂價設為 `Website`，您的網站可能會有不同的定價，也有後援預設定價值(請參閱 [價格範圍](https://experienceleague.adobe.com/docs/commerce-admin/catalog/products/pricing/catalog-price-scope.html))。

如果您將目錄價格範圍從 `Global` 至 `Website`，所有價格型別屬性也會變更為 `Website`. 另請參閱 [新增網站](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/stores.html#add-websites).

在選擇網站價格時，有兩個價格來源：

- 網站價格
- 預設（後退）價格

針對Amazon銷售管道整合，根據您的 [清單規則](./listing-rules.md)，您可以將多個網站的產品對應至單一網站 [!DNL Amazon Marketplace] 國家/地區(定義於 [存放區整合](./store-integration.md))。 不過，此對應會說明當產品存在於多個不同價格的網站時，應該發佈哪種價格的問題。
