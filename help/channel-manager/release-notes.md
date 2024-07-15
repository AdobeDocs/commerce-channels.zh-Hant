---
title: '[!DNL Channel Manager]發行說明'
description: Adobe Commerce中 [!DNL Channel Manager] 的最新發行資訊。
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# [!DNL Channel Manager]發行說明

這些版本說明說明[!DNL Channel Manager]的初始版本，包括：

![新](../assets/new.svg)新功能
![已修正問題](../assets/fix.svg)修正和改良
![已知問題](../assets/bug.svg)已知問題

請參閱[即將發行的版本](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html)，瞭解發行排程和支援。

請參閱[產品可用性](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html)，瞭解哪些Adobe Commerce版本支援此擴充功能。

## v2.1.0

*2023年10月3日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新](../assets/new.svg)頻道管理員現在與[Adobe Commerce 2.4.7版beta](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html)版本相容。

## v2.0.0

*2023年3月20日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新](../assets/new.svg)<!--CHAN-5893-->管道管理員現在與Adobe Commerce 2.4.6版相容。

## v1.1.0

*2022年11月23日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg)<!--CHAN-5204--> **退貨與退款** — 您現在可以處理透過Adobe Commerce和Magento Open Source Channel Manger商店出貨的訂單的Walmart Marketplace退貨與退款程式。 Walmart和Adobe Commerce之間會同步處理退貨和退款的資訊和更新，以便在[!DNL Commerce]店面和[!DNL Walmart Marketplace]中都能使用目前的資料。 請參閱[退貨和退款訂單](return-refund-orders.md)。

![已修正](../assets/fix.svg)<!--CHAN-5661-->修正使用`bin/magento saas:resync --feed orders`命令重新同步處理管道管理員訂單資料時發生的`Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist`錯誤。 透過更新銷售資料匯出程式模組的管道管理員套件相依性（已從`magento/module-sales-data-exporter`重新命名為`magento/module-sales-orders-data-exporter`）來解決錯誤。

## v1.0.0

*2022年1月14日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新](../assets/new.svg)頻道管理員的初始發行版本，以供一般使用

