---
title: 記錄和儲存報表
description: 使用記錄檔和儲存報表，查看Adobe商務或Magento Open Source商店以及Amazon Marketplace清單中發生的情況。
exl-id: 4654f718-d15f-4c3b-b984-ac7b9c29e6c4
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# 記錄和儲存報表

Amazon銷售管道擴充功能包含一些寶貴記錄和儲存報表，可讓您檢視影響Amazon清單和訂單的變更。 您可以使用這些報表來查看您商店中發生的狀況，並了解各種清單狀態。

記錄或儲存報表沒有可用的動作，因為這些是僅限檢閱的功能。

可以從[儲存儀表板](./amazon-store-dashboard.md)訪問以下日誌。

- [清單變更記錄](./listing-changes-log.md)顯示在您的Amazon賣家帳戶中發生的變更，以反映您的Amazon銷售管道設定。

- [通訊錯誤記錄](./communication-errors-log.md)會顯示任何回報的與Amazon的通訊錯誤。

可從[store dashboard](./amazon-store-dashboard.md)存取下列存放區特定報表。

- [競爭價格分析](./competitive-price-analysis.md)報表顯示您的Amazon _定價_（列價加運費）與[Buy Box](./buy-box-competitor-pricing.md)價格和[最低競爭者](./lowest-competitor-pricing.md)價格相關。

- [清單改善](./listing-improvements.md)報表顯示Amazon針對所選商店提供的所有建議清單改善。

>[!TIP]
>
>您也可以在需要進行疑難排解時，檢查記錄檔以取得其他資訊。 請參閱[銷售渠道管理設定](./sales-channel-settings.md)。 Amazon銷售渠道同步記錄寫入`{Commerce Root}/var/log/channel_amazon.log`檔案，可在[開發人員模式](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}中查看。
