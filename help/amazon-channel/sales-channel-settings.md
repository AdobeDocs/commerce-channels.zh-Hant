---
title: Sales Channel設定
description: 要管理Amazon銷售渠道功能的日誌記錄、克隆源和同步，請更新Commerce配置。
exl-id: 69f83774-41de-4fde-a357-f100d1bcd9f0
source-git-commit: 5508fe6e6b2193eaaebc78f485aae972504554cc
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Sales Channel設定

當 [!DNL Amazon Sales Channel] 已安裝擴展，在「Admin forAmazon銷售渠道」中設定預設值。 這些設定可在您的Amazon商店的配置設定中修改。 這些設定包括：

- 清除活動日誌歷史記錄的間隔
- Cron源選擇
- 日誌同步選項

## 修改Commerce Channels設定

1. 在 _管理_ 邊欄，轉到 **[!UICONTROL Stores]** > _[!UICONTROL Settings]_>**[!UICONTROL Configuration]**。

1. 在左面板中，展開 **[!UICONTROL Sales Channels]** 選擇 **[!UICONTROL Global Settings]**。

1. 對於 **[!UICONTROL Clear Log History]**，選擇選項：

   - `Once Daily`  — 選擇每天清除一次您的商店活動歷史記錄。

   - `Once Weekly`  — 選擇每週清除一次您的商店活動歷史記錄。

   - `Once Monthly`  — （預設）選擇每月清除一次您的儲存活動歷史記錄。

1. 對於 **[!UICONTROL Background Tasks (CRON) Source]**&#x200B;選項 `Magento CRON`。

   此選項允許Amazon銷售渠道使用 [!DNL Commerce] [克龍](https://docs.magento.com/user-guide/system/cron.html) 設定確定通信和資料同步間隔 [!DNL Amazon Seller Central]。

1. 對於 **[!UICONTROL Enable Debug Logging]**&#x200B;選項 `Enabled` 收集其他同步資料。

   Amazon銷售渠道日誌記錄寫入 `{Commerce Root}/var/log/channel_amazon.log` 可在 [開發者模式](https://docs.magento.com/user-guide/magento/installation-modes.html){target=&quot;_blank&quot;}。 日誌記錄應僅 `Enabled` 在故障排除期間，應 `Disabled` 完成故障排除。

1. 對於 **[!UICONTROL Read-Only Mode]**&#x200B;選中 `Enabled` 阻止所有傳出狀態更改API請求。

   使用此設定，在保存（但不發送）潛在更改之前 [!UICONTROL Read-Only Mode] 已禁用。 必須清除配置快取才能啟用只讀模式。 要再次啟動資料傳輸，請選擇 `Disabled`。

   >[!IMPORTANT]
   >
   >[!UICONTROL Read-Only Mode] 是為生產實例的副本而設計的，不應在生產實例上使用。
   >
   >當資料庫遷移到實例的新副本（當儲存的URL在配置中發生更改時檢測到）時， [!UICONTROL Read-Only Mode] 自動啟用。

1. 按一下 **[!UICONTROL Save Config]**.

![Sales Channel配置設定](assets/config-sales-channel-global-settings.png)
