---
title: 銷售管道設定
description: 若要管理Amazon銷售管道功能的記錄、cron來源和同步，請更新Commerce設定。
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
role: Admin, Developer
feature: Sales Channels, Configuration, Logs
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 銷售管道設定

安裝[!DNL Amazon Sales Channel]擴充功能後，會在Amazon銷售管道的「管理員」中設定預設值。 您可以在Amazon商店的組態設定中修改這些設定。 這些設定包括：

- 清除活動記錄記錄的間隔
- Cron來源選擇
- 記錄同步選項

## 修改Commerce頻道設定

1. 在&#x200B;_管理員_&#x200B;側邊欄上，移至&#x200B;**[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**。

1. 在左側面板中，展開&#x200B;**[!UICONTROL Sales Channels]**&#x200B;並選擇&#x200B;**[!UICONTROL Global Settings]**。

1. 針對&#x200B;**[!UICONTROL Clear Log History]**，選擇一個選項：

   - `Once Daily` — 選擇每天清除一次您的商店活動記錄。

   - `Once Weekly` — 選擇每週清除一次您的商店活動歷史記錄。

   - `Once Monthly` - （預設）選擇每月清除一次您的商店活動歷史記錄。

1. 針對&#x200B;**[!UICONTROL Background Tasks (CRON) Source]**，請選擇`Magento CRON`。

   此選項允許Amazon銷售管道使用您的[!DNL Commerce] [Cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)設定來決定與[!DNL Amazon Seller Central]的通訊和資料同步間隔。

1. 針對&#x200B;**[!UICONTROL Enable Debug Logging]**，選擇`Enabled`以在需要疑難排解時收集其他同步處理資料。

   Amazon sales channel記錄已寫入`{Commerce Root}/var/log/channel_amazon.log`檔案，且可在[開發人員模式](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/developer-tools.html#operation-modes)中檢視。 疑難排解期間，記錄只能是`Enabled`，疑難排解完成時應該是`Disabled`。

1. 針對&#x200B;**[!UICONTROL Read-Only Mode]**，選取`Enabled`以封鎖所有傳出狀態變更的API要求。

   使用此設定時，可能會儲存變更，但不會傳送，直到[!UICONTROL Read-Only Mode]停用為止。 必須清除設定快取，才能啟用唯讀模式。 若要再次開始資料傳輸，請選取`Disabled`。

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode]是為生產執行個體的復本而設計，例如測試或QA，不應該用於生產執行個體。
   >
   >當資料庫移轉至執行個體的新復本時（在組態中儲存區的URL變更時偵測），[!UICONTROL Read-Only Mode]會自動啟用。

1. 按一下&#x200B;**[!UICONTROL Save Config]**。

![Sales Channel組態設定](assets/config-sales-channel-global-settings.png){width="600" zoomable="yes"}
