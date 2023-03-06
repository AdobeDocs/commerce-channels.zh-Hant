---
title: Sales Channel設定
description: 若要管理Amazon銷售管道功能的記錄、登錄來源及同步，請更新Commerce設定。
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Sales Channel設定

當 [!DNL Amazon Sales Channel] 已安裝擴充功能，則會在「Amazon銷售管理」管道中設定預設值。 您可在Amazon商店的組態設定中修改這些設定。 這些設定包括：

- 清除活動日誌歷史記錄的間隔
- Cron源選擇
- 日誌同步選項

## 修改「商務」管道設定

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**.

1. 在左側面板中，展開 **[!UICONTROL Sales Channels]** 選擇 **[!UICONTROL Global Settings]**.

1. 針對 **[!UICONTROL Clear Log History]**，選擇選項：

   - `Once Daily`  — 選擇每天清除一次您的商店活動歷史記錄。

   - `Once Weekly`  — 選擇每週清除一次您的商店活動歷史記錄。

   - `Once Monthly`  — （預設）選擇每月清除一次您的商店活動歷史記錄。

1. 針對 **[!UICONTROL Background Tasks (CRON) Source]**，選擇 `Magento CRON`.

   此選項可讓Amazon銷售管道使用 [!DNL Commerce] [Cron](https://docs.magento.com/user-guide/system/cron.html) 確定通信和資料同步間隔的設定 [!DNL Amazon Seller Central].

1. 針對 **[!UICONTROL Enable Debug Logging]**，選擇 `Enabled` 以在需要進行故障排除時收集其他同步資料。

   Amazon銷售管道記錄會寫入 `{Commerce Root}/var/log/channel_amazon.log` 檔案和可在 [開發人員模式](https://docs.magento.com/user-guide/magento/installation-modes.html){target="_blank"}. 記錄應僅 `Enabled` 進行疑難排解時，應該 `Disabled` 疑難排解完成時。

1. 針對 **[!UICONTROL Read-Only Mode]**，選取 `Enabled` 來封鎖所有傳出狀態變更API請求。

   使用此設定，在 [!UICONTROL Read-Only Mode] 已停用。 必須清除配置快取，才能啟用只讀模式。 若要重新開始資料傳輸，請選取 `Disabled`.

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] 專為生產執行個體的復本（例如測試或QA）而設計，不應用於生產執行個體。
   >
   >將資料庫遷移到實例的新副本時（當配置中儲存的URL更改時檢測到）, [!UICONTROL Read-Only Mode] 會自動啟用。

1. 按一下 **[!UICONTROL Save Config]**.

![Sales Channel配置設定](assets/config-sales-channel-global-settings.png)
