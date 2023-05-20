---
title: '"[!DNL Channel Manager] 發行說明'''
description: 的最新發佈資訊 [!DNL Channel Manager] Adobe Commerce。
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: d3acde7aa297ba33dffa7854aa7578985ad12c9b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# [!DNL Channel Manager] 發行說明

本發行說明描述了 [!DNL Channel Manager] 包括：

![新建](../assets/new.svg) 新功能
![已修復問題](../assets/fix.svg) 修復和改進
![已知問題](../assets/bug.svg) 已知問題


## v2.0.0

*2023年3月20日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新建](../assets/new.svg)<!--CHAN-5893--> Channel Manager現在與Adobe Commerce2.4.6版相容。

## v1.1.0

*2022年11月23日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新建](../assets/new.svg)<!--CHAN-5204--> **退貨和退款** — 您現在可以處理通過Adobe Commerce和Magento Open Source渠道管理商店發運的訂單的Walmart Marketplace退貨和退款流程。 有關退貨和退款的資訊和更新會在沃爾瑪和Adobe Commerce之間同步，以便當前資料可在 [!DNL Commerce] 店面 [!DNL Walmart Marketplace]。 請參閱 [退貨和退款訂單](return-refund-orders.md)。

![固定](../assets/fix.svg)<!--CHAN-5661--> 已修復 `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` 重新同步Channel Manager時使用 `bin/magento saas:resync --feed orders` 的子菜單。 通過更新銷售資料導出器模組的Channel Manager包依賴項解決了該錯誤，該模組已從 `magento/module-sales-data-exporter` 至 `magento/module-sales-orders-data-exporter`。

## v1.0.0

*2022年1月14日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新建](../assets/new.svg) Channel Manager的初始版本，以實現全面可用性

