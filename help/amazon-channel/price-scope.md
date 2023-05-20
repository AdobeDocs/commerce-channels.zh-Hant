---
title: 價格範圍
description: 使用Commerce定價範圍可以根據多個網站或全球範圍管理定價。
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# 價格範圍

[!DNL Commerce] 提供配置 [定價範圍](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} to be set to `Global` or `Website`. If pricing is set to `Global`, there is a single price source for all websites. If pricing is set to `Website`, your websites can vary their pricing across and also have a fallback default pricing value. See [Catalog Price](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){target="_blank"} 中。

如果更改目錄價格範圍 `Global` 至 `Website`，所有價格類型屬性也更改為 `Website`。 請參閱 [添加網站](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){target="_blank"}。

選擇網站價格時，有兩種價格來源：

- 網站價格
- 預設（回落）價格

對於Amazon銷售渠道整合，根據您 [上市規則](./listing-rules.md)，您可以將多個網站的產品映射到單個網站 [!DNL Amazon Marketplace] 國家(在 [儲存整合](./store-integration.md))。 但是，此映射引入了如果產品存在於價格不同的多個網站上，應發佈價格的問題。
