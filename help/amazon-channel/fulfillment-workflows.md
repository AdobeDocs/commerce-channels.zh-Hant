---
title: Amazon完成工作流程
description: 從Amazon清單完成訂單會遵循從訂單提交到發運的特定順序。
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon完成工作流程

## 範例：由商戶履行

| 步驟 | 說明 |
|----|----|
| 3 | **商戶履行的訂單會在Amazon上下。** Amazon會指派狀態 `Pending` ，直到客戶的信用卡資訊經驗證為止。處於`Pending`狀態的訂單會自動匯入至Amazon銷售管道，但不會顯示在&#x200B;_[!UICONTROL Orders]_標籤上。 |
| 2 | **訂單經Amazon驗證。** 驗證後，Amazon會將狀態變更為 `Unshipped`。此狀態變更後，訂單會在Amazon銷售管道中更新，並顯示在&#x200B;_[!UICONTROL Orders]_標籤中。 |
| 3 | **訂單詳細資訊會更新。** Amazon銷售管道會以價格、客戶電子郵件和客戶名稱更新訂單詳細資訊。在此更新期間，Amazon訂單會在訂單管理頁面中建立對應的[!DNL Commerce]訂單。 [!DNL Commerce]訂單編號隨訂單資訊一起顯示在&#x200B;_[!UICONTROL Orders]_頁簽上。 |
| 4 | **已建立新客戶帳戶。** 如果您在訂單設定中進行設定，且您的資料庫中不 [!DNL Commerce] 存在客戶，則會使用Amazon訂單中 [!DNL Commerce] 對應的客戶資訊，在您的資料庫中建立新客戶。如果您在訂單設定中選擇了`No Customer Creation (guest)`，則訂單將遵循[!DNL Commerce]來賓流程，而不是在資料庫中建立客戶。 此時，如果您的[!DNL Commerce]系統與ERP/OMS/WMS整合，則會根據[!DNL Commerce]內放置並建立的新訂單的整合來提取訂單。 |
| 5 | **訂單已發運。** 從訂 [!DNL Commerce] 單處理頁面，您發運訂單並新增追蹤編號。當所有項都標籤為`Shipped`狀態時：<ul><li>[!DNL Commerce]順序的狀態將更改為`Complete`。</li><li>Amazon銷售渠道訂單的狀態將更改為`Shipped`。</li><li>追蹤號碼會同步至Amazon，而Amazon中的順序狀態會變更為`Shipped`。</li><li>運送通知會透過Amazon傳送給客戶，而非從[!DNL Commerce](根據Amazon的政策)傳送。 |

## 範例：由Amazon(FBA)履行

| 步驟 | 說明 |
|---|---|
| 3 | **Amazon履行的訂單會在Amazon上下。** |
| 2 | **訂單已匯入。** 在由Amazon指派訂單狀態之前，訂單不會匯入至Amazon `Shipped` 銷售管道。由於Amazon有此產品的庫存，因此可防止干擾您的倉庫/庫存管理。 |
| 3 | **訂單詳細資訊會更新。** 如果已在您的 [訂單設定](./order-settings.md)中進行設定，Amazon訂單會建 [!DNL Commerce] 立對應的訂單，並以狀態為的訂單來建 `Complete`立。 |
