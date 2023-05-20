---
title: Amazon商店視圖
description: 轉至「Amazon商店」視圖，快速查看每個Amazon商店的基本統計資訊和訪問管理選項。
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Amazon商店視圖

查看Amazon銷售渠道首頁時， _Amazon商店_ 視圖預設開啟。

![Amazon商店視圖](assets/amazon-sales-channel-home-tabs.png)

的 _[!UICONTROL Amazon Stores]_「view（視圖）」顯示您的每個Amazon商店的「儲存卡」以及一些基本統計和管理選項。 每張卡中顯示的摘要資訊包括每個儲存狀態、建立日期、上次更新日期、需要注意的清單(例如：未完成清單)和分配的 [!DNL Commerce] 的子菜單。

查看 _[!UICONTROL Amazon Store]_查看，每個儲存卡允許您：

- 開啟商店 [儀表板](./amazon-store-dashboard.md)按一下 **[!UICONTROL View Store]**。

- 要更改儲存狀態或刪除儲存，請按一下 **[!UICONTROL Action]** ，然後選擇：

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]**  — 選擇將儲存的狀態更改為 `Active` 或 `Inactive`的下界。

      更改 `Inactive` 儲存 `Active` 狀態使用商店當前的商店設定（如清單設定、價格規則和覆蓋）激活商店的清單和訂單活動。

      更改儲存狀態 `Active` 至 `Inactive` 狀態掛起儲存的清單和訂單活動。 非活動儲存保留所有儲存設定和清單，但暫時停止定價、數量和訂單管理的同步，直到將儲存更改回 `Active` 狀態。 此功能允許您在區域級別控制您的商店活動，而無需重新建立或重新整合您的Amazon商店或丟失歷史訂單和銷售資料。

   - **[!UICONTROL Delete]**  — 選擇刪除不再需要的儲存。

      選擇要刪除現有的Amazon商店及其與您的 [!DNL Amazon Seller Central] 帳戶。 刪除帳戶會從Amazon銷售渠道刪除該商店，以及所有帳戶設定、清單、日誌和與此商店相關的其他資訊。 刪除後無法檢索儲存，必須建立新儲存。

>[!NOTE]
>要在整合期間更改分配給儲存的網站，必須刪除儲存並使用在儲存整合期間定義的不同網站再次添加儲存。

| 儲存卡 | 說明 |
|--- |--- |
| 頂部 | 包括： <br>儲存區域表徵圖，在 [儲存整合](./store-integration.md)。<br> 已分配 _[!UICONTROL Magento Website]_，在儲存整合過程中定義。<br>的_[!UICONTROL Status]_ 你店裡的。 選項： **[!UICONTROL Active]**  — 商店整合已完成並經Amazon驗證，可用於銷售活動。 **[!UICONTROL Inactive]**  — 商店整合已完成，但尚未使用或可用於銷售活動。 當 `Inactive`，您的Amazon銷售暫停。 當 `Active`，在激活前保存銷售收入和其他設定以進行更新。<br>的 *[!UICONTROL Last Updated]* 最近更改Amazon商店設定的日期。<br>的 *[!UICONTROL Created]* Amazon商店在Amazon銷售渠道中建立的日期。 |
| 中段 | 包括過去30天的儲存活動摘要圖表，並包括需要注意的所有清單並發出警報。 |
| 底部 | 包括「查看儲存」和「操作」選項。<br>開啟商店 [儀表板](./amazon-store-dashboard.md)按一下 **[!UICONTROL View Store]**。<br>要激活、停用或刪除儲存，請按一下 **[!UICONTROL Actions]**。 |
