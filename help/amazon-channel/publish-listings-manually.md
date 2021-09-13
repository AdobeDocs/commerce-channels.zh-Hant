---
title: 手動發佈Amazon清單
description: 需要時，您可以向商務管理員手動發佈已結束的Amazon清單。
exl-id: ca3f674e-d93a-44a6-8c06-b417694a0f1e
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# 手動發佈Amazon清單

您可以手動發佈一或多個已結束的Amazon清單。

1. 在[產品清單](./managing-product-listings.md)頁（_[!UICONTROL Inactive]_、_[!UICONTROL Active]_&#x200B;或&#x200B;_[!UICONTROL Ineligible]_頁簽）的_[!UICONTROL Ended]_&#x200B;頁簽上查看一個或多個清單。

1. 在左欄中，按一下以勾選您要重新發佈的每個清單。

1. 在&#x200B;_[!UICONTROL Actions]_下，按一下&#x200B;**[!UICONTROL Publish Product to Amazon]**。

1. 按一下確認訊息中的&#x200B;**[!UICONTROL OK]**。

   系統會顯示訊息，確認正在處理選取的清單以發佈至Amazon。

   清單資訊會根據您的cron設定發佈至Amazon。 清單資訊會在下次資料同步時傳送至Amazon。 在Amazon以清單確認回覆之前，手動發佈的清單會保留在狀態為`List in Progress`的&#x200B;_準備列出_&#x200B;標籤上。 從Amazon收到清單確認時，清單會移至狀態為`Active`的&#x200B;_Active_&#x200B;標籤。
