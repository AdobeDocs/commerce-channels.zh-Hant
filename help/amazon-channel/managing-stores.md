---
title: Amazon商店檢視
description: 前往「Amazon商店」檢視，快速檢閱每個Amazon商店的基本統計資料和存取管理選項。
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Amazon商店檢視

檢視Amazon銷售管道首頁時， _Amazon商店_ 視圖預設會開啟。

![Amazon商店檢視](assets/amazon-sales-channel-home-tabs.png)

此 _[!UICONTROL Amazon Stores]_檢視會顯示每個Amazon商店的「商店卡」，以及一些基本統計資料和管理選項。 每張卡片中顯示的摘要資訊包括每個商店狀態、建立日期、上次更新日期、需要注意的清單(例如：未完成清單)和已分配 [!DNL Commerce] 網站。

檢視 _[!UICONTROL Amazon Store]_檢視，每張商店卡可讓您：

- 開店 [儀表板](./amazon-store-dashboard.md)，按一下 **[!UICONTROL View Store]**.

- 要更改儲存狀態或刪除儲存，請按一下 **[!UICONTROL Action]** 並選擇：

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]**  — 選擇將儲存狀態更改為 `Active` 或 `Inactive`，分別為。

      變更 `Inactive` 儲存至 `Active` 狀態會使用商店目前的商店設定（例如清單設定、價格規則和覆蓋）來啟用商店的清單和訂單活動。

      將儲存狀態從 `Active` to `Inactive` 狀態會暫停商店的清單和訂單活動。 非活動儲存保留所有儲存設定和清單，但暫時停止定價、數量和訂單管理的同步，直到將儲存更改回 `Active` 狀態。 此功能可讓您在地區層級控制您的商店活動，而無需重新建立或重新整合您的Amazon商店，或遺失歷史訂單和銷售資料。

   - **[!UICONTROL Delete]**  — 選擇刪除不再需要的儲存。

      選擇您要刪除現有Amazon商店及其與 [!DNL Amazon Seller Central] 帳戶。 刪除帳戶會從Amazon銷售管道中移除該商店，以及所有帳戶設定、清單、日誌和與此商店相關的其他資訊。 刪除後無法檢索儲存，必須建立新儲存。

>[!NOTE]
>若要在整合期間變更指派給商店的網站，您必須刪除商店，並使用商店整合期間定義的不同網站再次新增商店。

| 儲存卡 | 說明 |
|--- |--- |
| 頂端區段 | 包括： <br>商店的地區圖示，在 [商店整合](./store-integration.md).<br> 指派的 _[!UICONTROL Magento Website]_，在商店整合期間定義。<br>此_[!UICONTROL Status]_ 你的店。 選項： **[!UICONTROL Active]**  — 商店整合已完成，並已透過Amazon驗證，且可供銷售活動使用。 **[!UICONTROL Inactive]**  — 商店整合已完成，但未使用或可供銷售活動使用。 當 `Inactive`，您的Amazon銷售會暫停。 當 `Active`、銷售收入和其他設定儲存以在啟用前更新。<br>此 *[!UICONTROL Last Updated]* Amazon商店設定最新變更的日期。<br>此 *[!UICONTROL Created]* 在Amazon銷售管道中建立Amazon商店的日期。 |
| 中段 | 包括最近30天的商店活動摘要圖表，並包括需要注意的任何清單的和警報。 |
| 底部 | 包含「檢視儲存」和「動作」選項。<br>開啟商店 [儀表板](./amazon-store-dashboard.md)，按一下 **[!UICONTROL View Store]**.<br>若要啟用、停用或刪除商店，請按一下 **[!UICONTROL Actions]**. |
