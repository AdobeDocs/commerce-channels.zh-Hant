---
title: Amazon商店檢視
description: 前往「Amazon商店」檢視，快速檢閱每個Amazon商店的基本統計資料和存取管理選項。
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Amazon商店檢視

檢視Amazon銷售管道首頁時，預設會開啟&#x200B;_Amazon商店_&#x200B;檢視。

![Amazon商店檢視](assets/amazon-sales-channel-home-tabs.png)

_[!UICONTROL Amazon Stores]_檢視會顯示每個Amazon商店的「商店卡」，以及一些基本統計資料和管理選項。 每張卡片中顯示的摘要資訊包括每個商店狀態、建立日期、上次更新日期、需要注意的清單(例如：未完成清單)和指派的[!DNL Commerce]網站。

檢視&#x200B;_[!UICONTROL Amazon Store]_檢視時，每個商店卡可讓您：

- 若要開啟商店[儀表板](./amazon-store-dashboard.md)，請按一下&#x200B;**[!UICONTROL View Store]**。

- 要更改儲存狀態或刪除儲存，請按一下&#x200B;**[!UICONTROL Action]**&#x200B;並選擇：

   - **[!UICONTROL Activate]** /  **[!UICONTROL Deactivate]**  — 選擇將儲存狀態分別變 `Active` 更 `Inactive`為或。

      將`Inactive`商店變更為`Active`狀態會使用商店目前的商店設定（如清單設定、價格規則和覆蓋）來啟用商店的清單和訂單活動。

      將儲存狀態從`Active`變更為`Inactive`會暫停該儲存的清單和訂購活動。 非活動儲存保留所有儲存設定和清單，但暫時停止定價、數量和訂單管理的同步，直到將儲存更改回`Active`狀態。 此功能可讓您在地區層級控制您的商店活動，而無需重新建立或重新整合您的Amazon商店，或遺失歷史訂單和銷售資料。

   - **[!UICONTROL Delete]**  — 選擇刪除不再需要的儲存。

      選擇您要刪除現有Amazon商店及其與[!DNL Amazon Seller Central]帳戶的整合設定的時間。 刪除帳戶會從Amazon銷售管道中移除該商店，以及所有帳戶設定、清單、日誌和與此商店相關的其他資訊。 刪除後無法檢索儲存，必須建立新儲存。

>[!NOTE]
>若要在整合期間變更指派給商店的網站，您必須刪除商店，並使用商店整合期間定義的不同網站再次新增商店。

| 儲存卡 | 說明 |
|--- |--- |
| 頂端區段 | 包括：<br>商店整合](./store-integration.md)期間定義的商店區域圖示。[<br> 指派的， _[!UICONTROL Magento Website]_在儲存整合期間定義。<br>你_[!UICONTROL Status]_ 店的。選項：**[!UICONTROL Active]** — 商店整合已完成，並已透過Amazon驗證，且可供銷售活動使用。 **[!UICONTROL Inactive]**  — 商店整合已完成，但未使用或可供銷售活動使用。`Inactive`時，您的Amazon銷售暫停。 `Active`時，銷售收入和其他設定會儲存以在啟動前更新。<br>Amazon *[!UICONTROL Last Updated]* 商店設定的最新變更日期。<br>在 *[!UICONTROL Created]* Amazon銷售管道中建立Amazon商店的日期。 |
| 中段 | 包括最近30天的商店活動摘要圖表，並包括需要注意的任何清單的和警報。 |
| 底部 | 包含「檢視儲存」和「動作」選項。<br>若要開啟存放區控 [制面板](./amazon-store-dashboard.md)，請按一下 **[!UICONTROL View Store]**。<br>若要啟用、停用或刪除商店，請按一下「 」 **[!UICONTROL Actions]**。 |
