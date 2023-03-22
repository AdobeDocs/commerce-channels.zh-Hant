---
title: '[!DNL Channel Manager] 發行說明'
description: 的最新發行資訊 [!DNL Channel Manager] 從Adobe Commerce。
exl-id: 8f40ace1-6587-4185-955a-91bc16dee8ce
source-git-commit: 9cc1b79089771ef9a58d22379197b210d31e1670
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# [!DNL Channel Manager] 發行說明

以下版本說明的初始版本 [!DNL Channel Manager] 包括：

![新增](../assets/new.svg) 新功能
![修正問題](../assets/fix.svg) 修正和改良
![已知問題](../assets/bug.svg) 已知問題


## v1.1.0

![新增](../assets/new.svg)<!--CHAN-5204--> **退貨與退款** — 您現在可以處理通過Adobe Commerce和Magento Open Source渠道經理商店發運的訂單的Walmart Marketplace退貨和退款流程。 有關退貨和退款的資訊和更新會在沃爾瑪和Adobe Commerce之間同步，以便在 [!DNL Commerce] 店面 [!DNL Walmart Marketplace]. 請參閱 [退貨和退貨訂單](return-refund-orders.md).

![固定](../assets/fix.svg)<!--CHAN-5661--> 修正 `Class Magento\SalesDataExporter\MOdel\OrdersFeed does not exist` 重新同步Channel Manager時，使用 `bin/magento saas:resync --feed orders` 命令。 更新銷售資料導出器模組的渠道管理器包依賴項(已從 `magento/module-sales-data-exporter` to `magento/module-sales-orders-data-exporter`.

## v1.0.0

初始發行，與下列商務版本相容：

* 開放原始碼(CE):2.4.x
* Adobe Commerce(EE):2.4.x
* Adobe Commerce for Cloud(ECE):2.4.x
* 穩定性：穩定
