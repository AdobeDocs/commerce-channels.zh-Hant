---
title: Sales Channel設定
description: 若要管理Amazon銷售管道功能的記錄、登錄來源及同步，請更新Commerce設定。
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Sales Channel設定

安裝[!DNL Amazon Sales Channel]擴充功能時，會在「Amazon銷售管道管理員」中設定預設值。 您可在Amazon商店的組態設定中修改這些設定。 這些設定包括：

- 清除活動日誌歷史記錄的間隔
- Cron源選擇
- 日誌同步選項

## 修改「商務」管道設定

1. 在&#x200B;_Admin_&#x200B;側欄中，前往&#x200B;**[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**。

1. 在左側面板中，展開&#x200B;**[!UICONTROL Sales Channels]**&#x200B;並選擇&#x200B;**[!UICONTROL Global Settings]**。

1. 對於&#x200B;**[!UICONTROL Clear Log History]**，選擇一個選項：

   - `Once Daily`  — 選擇每天清除一次您的商店活動歷史記錄。

   - `Once Weekly`  — 選擇每週清除一次您的商店活動歷史記錄。

   - `Once Monthly`  — （預設）選擇每月清除一次您的商店活動歷史記錄。

1. 對於&#x200B;**[!UICONTROL Background Tasks (CRON) Source]**，選擇`Magento CRON`。

   此選項可讓Amazon銷售管道使用您的[!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html)設定，以判斷與[!DNL Amazon Seller Central]的通訊和資料同步間隔。

1. 對於&#x200B;**[!UICONTROL Enable Debug Logging]**，選擇`Enabled`以在需要進行故障排除時收集其他同步資料。

   Amazon銷售管道記錄會寫入`{Commerce Root}/var/log/channel_amazon.log`檔案中，並可在[開發人員模式](https://docs.magento.com/user-guide/magento/installation-modes.html){:target=&quot;_blank&quot;}中檢視。 疑難排解期間記錄應僅為`Enabled`，完成疑難排解時應為`Disabled`。

1. 按一下&#x200B;**[!UICONTROL Save Config]**。

![Sales Channel配置設定](assets/config-sales-channel-global-settings.png)
