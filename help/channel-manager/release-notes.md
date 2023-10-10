---
title: '[!DNL Channel Manager] 發行說明'
description: 的最新版本資訊 [!DNL Channel Manager] 來自Adobe Commerce。
feature: Sales Channels, Release Notes
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 003efd3c1044284a7d2c86db5d3eb1abfb3898ea
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 3%

---

# [!DNL Channel Manager] 發行說明

以下版本說明說明的初始版本 [!DNL Channel Manager] 並包含：

![新增](../assets/new.svg) 新功能
![已修正的問題](../assets/fix.svg) 修正和改良
![已知問題](../assets/bug.svg) 已知問題

另請參閱 [即將發行的版本](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) 以瞭解發行排程和支援。

另請參閱 [產品可用性](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) 以瞭解哪些Adobe Commerce版本支援此擴充功能。

## v2.1.0

*2023年10月3日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) Channel Manager現在相容於 [Adobe Commerce 2.4.7版Beta版](https://experienceleague.adobe.com/docs/commerce-operations/release/beta.html) 發行版本。

## v2.0.0

*2023年3月20日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg)<!--CHAN-5893--> Channel Manager現在與Adobe Commerce 2.4.6版相容。

## v1.1.0

*2022年11月23日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg)<!--CHAN-5204--> **退貨與退款** — 您現在可以處理透過Adobe Commerce和Magento Open Source Channel Manger商店出貨的訂單的Walmart Marketplace退貨與退款程式。 有關退貨和退款的資訊和更新會在Walmart和Adobe Commerce之間同步，以便可以在以下兩個頁面取得目前的資料： [!DNL Commerce] 店面和 [!DNL Walmart Marketplace]. 另請參閱 [退貨與退款訂單](return-refund-orders.md).

![固定](../assets/fix.svg)<!--CHAN-5661--> 已修正 `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` 使用重新同步處理管道管理員訂單資料時發生錯誤 `bin/magento saas:resync --feed orders` 命令。 透過更新銷售資料匯出工具模組的管道管理員套件相依性(已重新命名為 `magento/module-sales-data-exporter` 至 `magento/module-sales-orders-data-exporter`.

## v1.0.0

*2022年1月14日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) Channel Manager初次發行正式發行

