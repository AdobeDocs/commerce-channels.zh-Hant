---
title: Amazon清單的記錄和商店報告
description: 使用記錄檔和商店報告來檢視您的Adobe Commerce或Magento Open Source商店發生什麼事，以及您的Amazon Marketplace清單。
feature: Sales Channels, Logs
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Amazon清單的記錄和商店報告

Amazon Sales Channel擴充功能包括一些重要的記錄和商店報表，可讓您檢視影響Amazon清單和訂單的變更。 您可以使用這些報表來檢視商店中正在發生的事情，並瞭解各種清單狀態。

沒有可用於記錄或存放區報告的動作，因為它們是僅限檢閱的功能。

下列記錄檔可從 [存放區儀表板](./amazon-store-dashboard.md).

- 此 [列出變更記錄](./listing-changes-log.md) 顯示在您的Amazon賣家帳戶中發生的變更，以反映您的Amazon銷售管道設定。

- 此 [通訊錯誤記錄](./communication-errors-log.md) 顯示與Amazon之間任何回報的通訊錯誤。

下列商店特定報表可從下列網址存取： [存放區儀表板](./amazon-store-dashboard.md).

- 此 [具競爭力的價格分析](./competitive-price-analysis.md) 報表顯示您的Amazon _起岸價格_ （上市價格加運費）與 [Buy Box](./buy-box-competitor-pricing.md) 價格與 [最低競爭者](./lowest-competitor-pricing.md) 價格。

- 此 [清單改善](./listing-improvements.md) 報表會顯示Amazon為選取的商店提供的所有建議清單改善。

>[!TIP]
>
>如需疑難排解的其他資訊，您也可以檢視記錄檔。 另請參閱 [sales channel管理員設定](./sales-channel-settings.md). Amazon sales channel同步記錄會寫入 `{Commerce Root}/var/log/channel_amazon.log` 檔案及檢視位置 [開發人員模式](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes).
