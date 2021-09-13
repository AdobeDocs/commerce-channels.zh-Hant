---
title: 價格範圍
description: 使用商務定價範圍根據多個網站或全球管理定價。
exl-id: 24a1eac1-d579-4063-a33c-71969bc2b4b9
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# 價格範圍

[!DNL Commerce] 提供要設 [定為或的定價範圍](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;} `Global` 的設定 `Website`。如果定價設為`Global`，則所有網站都有單一價格來源。 如果定價設為`Website`，則您的網站可能會因價格而異，且也會有後援的預設定價值。 請參閱核心商務使用手冊中的[目錄價格](https://docs.magento.com/user-guide/configuration/catalog/catalog.html#price){:target=&quot;_blank&quot;}。

如果將目錄價格範圍從`Global`更改為`Website`，則所有價格類型屬性也將更改為`Website`。 請參閱[新增網站](https://docs.magento.com/user-guide/stores/stores-all-create-website.html){:target=&quot;_blank&quot;}。

選擇網站價格時，有兩個價格來源：

- 網站價格
- 預設（回落）價格

對於Amazon銷售管道整合，您可以根據您的[清單規則](./listing-rules.md)，將多個網站的產品對應至單一[!DNL Amazon Marketplace]國家（在[商店整合](./store-integration.md)期間定義）。 不過，此對應會介紹如果產品存在於價格不同的多個網站上，則應發佈價格的問題。
