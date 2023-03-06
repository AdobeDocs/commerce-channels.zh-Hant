---
title: 價格範圍
description: 使用商務定價範圍根據多個網站或全球管理定價。
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 價格範圍

[!DNL Commerce] 提供 [定價範圍](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} to be set to `Global` or `Website`. If pricing is set to `Global`, there is a single price source for all websites. If pricing is set to `Website`, your websites can vary their pricing across and also have a fallback default pricing value. See [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} （在核心商務使用手冊中）。

如果您將目錄價格範圍從 `Global` to `Website`，所有價格類型屬性也會變更為 `Website`. 請參閱 [新增網站](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target="_blank"}.

選擇網站價格時，有兩個價格來源：

- 網站價格
- 預設（回落）價格

針對Amazon銷售管道整合，根據 [清單規則](./listing-rules.md)，您可以將來自多個網站的產品對應至單一 [!DNL Amazon Marketplace] 國家(定義於 [商店整合](./store-integration.md))。 不過，此對應會介紹如果產品存在於價格不同的多個網站上，則應發佈價格的問題。
