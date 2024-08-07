---
title: '[!UICONTROL Amazon Stores]檢視'
description: 前往Amazon商店檢視，快速檢閱每個Amazon商店的基本統計資料，以及存取管理選項。
feature: Sales Channels, Storefront
exl-id: 1376cd84-da81-4d3b-a5be-218aa802eed6
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# [!UICONTROL Amazon Stores]檢視

檢視Amazon銷售管道首頁時，_Amazon商店_&#x200B;檢視預設會開啟。

![Amazon商店檢視](assets/amazon-sales-channel-home-tabs.png){width="600" zoomable="yes"}

_[!UICONTROL Amazon Stores]_檢視會顯示每個Amazon商店的「商店卡」，以及一些基本統計和管理選項。 每張卡片中所顯示的摘要資訊包含每個商店狀態、建立日期、上次更新日期、需要注意的清單（例如：未完成的清單）以及指派的[!DNL Commerce]網站。

檢視&#x200B;_[!UICONTROL Amazon Store]_檢視時，每個商店卡可讓您：

- 若要開啟商店[儀表板](./amazon-store-dashboard.md)，請按一下&#x200B;**[!UICONTROL View Store]**。

- 若要變更商店狀態或刪除商店，請按一下&#x200B;**[!UICONTROL Action]**&#x200B;並選擇：

   - **[!UICONTROL Activate]** / **[!UICONTROL Deactivate]** — 選擇將存放區的狀態分別變更為`Active`或`Inactive`。

     將`Inactive`商店變更為`Active`狀態會使用商店目前的商店設定（例如清單設定、價格規則和覆寫）來啟動商店的清單和訂購活動。

     將商店狀態從`Active`變更為`Inactive`會暫停商店的清單和訂購活動。 非使用中存放區會保留所有存放區設定和清單，但會暫時停止訂價、數量及訂單管理的同步處理，直到存放區變更回`Active`狀態為止。 此功能可讓您在地區層級控制商店活動，而不需要重新建立或重新整合您的Amazon商店，或遺失歷史訂單和銷售資料。

   - **[!UICONTROL Delete]** — 選擇刪除不再需要的存放區。

     選擇您要刪除現有Amazon存放區及其與[!DNL Amazon Seller Central]帳戶的整合設定的時間。 刪除帳戶會從Amazon銷售管道移除商店，以及與此商店相關的所有帳戶設定、清單、記錄及其他資訊。 刪除後無法擷取存放區，必須建立新存放區。

>[!NOTE]
>若要在整合期間變更指派給商店的網站，您必須刪除商店，然後使用商店整合期間定義的不同網站再次新增商店。

| 商店卡片 | 說明 |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 頂端區段 | 包含： <br>存放區的區域圖示，定義於[存放區整合](./store-integration.md)。<br>指派的&#x200B;_[!UICONTROL Magento Website]_，在存放區整合期間定義。<br>您商店的_[!UICONTROL Status]_。 選項： **[!UICONTROL Active]** — 商店整合已完成，並已透過Amazon驗證，可供銷售活動使用。 **[!UICONTROL Inactive]** — 商店整合已完成，但並未使用或可供銷售活動使用。 當`Inactive`時，會暫停您的Amazon銷售。 當`Active`時，銷售收入和其他設定會儲存以在啟用之前更新。<br>最近變更Amazon市集設定的&#x200B;*[!UICONTROL Last Updated]*&#x200B;日期。<br>在Amazon銷售管道中建立Amazon商店的&#x200B;*[!UICONTROL Created]*&#x200B;日期。 |
| 中段 | 包含過去30天的商店活動摘要圖表，並包含任何需要注意的清單和警報。 |
| 底部區段 | 包含檢視存放區和動作選項。<br>若要開啟存放區[儀表板](./amazon-store-dashboard.md)，請按一下&#x200B;**[!UICONTROL View Store]**。<br>若要啟用、停用或刪除存放區，請按一下&#x200B;**[!UICONTROL Actions]**。 |
