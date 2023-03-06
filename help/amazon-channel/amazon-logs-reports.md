---
title: 記錄和儲存報表
description: 使用記錄檔和儲存報表，查看Adobe Commerce或Magento Open Source存放區以及Amazon Marketplace清單中發生的情況。
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 記錄和儲存報表

Amazon銷售管道擴充功能包含一些寶貴記錄和儲存報表，可讓您檢視影響Amazon清單和訂單的變更。 您可以使用這些報表來查看您商店中發生的狀況，並了解各種清單狀態。

記錄或儲存報表沒有可用的動作，因為這些是僅限檢閱的功能。

下列記錄檔可從 [儲存儀表板](./amazon-store-dashboard.md).

- 此 [列出更改日誌](./listing-changes-log.md) 顯示在您的Amazon賣家帳戶中發生的變更，以反映您的Amazon銷售管道設定。

- 此 [通信錯誤日誌](./communication-errors-log.md) 顯示任何回報的與Amazon的通訊錯誤。

下列存放區特定報表可透過 [儲存儀表板](./amazon-store-dashboard.md).

- 此 [競爭價格分析](./competitive-price-analysis.md) 報表顯示您的Amazon _定價_ （上市價加運費）。 [Buy Box](./buy-box-competitor-pricing.md) 價格和 [最低競爭者](./lowest-competitor-pricing.md) 價格。

- 此 [清單改善](./listing-improvements.md) 報表顯示Amazon針對所選商店提供的所有建議清單改善項目。

>[!TIP]
>
>您也可以在需要進行疑難排解時，檢查記錄檔以取得其他資訊。 請參閱 [銷售管道管理員設定](./sales-channel-settings.md). Amazon銷售渠道同步記錄將寫入 `{Commerce Root}/var/log/channel_amazon.log` 檔案和可在 [開發人員模式](https://docs.magento.com/user-guide/magento/installation-modes.html){target="_blank"}.
