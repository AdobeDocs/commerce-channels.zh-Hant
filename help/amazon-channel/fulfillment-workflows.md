---
title: Amazon履行工作流
description: 從Amazon清單完成訂單後，將按照從提交訂單到發運的特定順序執行。
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon履行工作流

## 示例：商人履行

| 步驟 | 說明 |
|----|----|
| 1 | **商人履行的訂單被下達到Amazon。** Amazon為 `Pending` 直到驗證客戶的信用卡資訊。 訂單 `Pending` 狀態自動導入到Amazon銷售渠道，但不顯示在 _[!UICONTROL Orders]_頁籤。 |
| 2 | **命令由Amazon覈實。** 驗證後，Amazon將狀態更改為 `Unshipped`。 在此狀態更改後，訂單將在Amazon銷售渠道中更新，並出現在 _[!UICONTROL Orders]_頁籤。 |
| 3 | **訂單詳細資訊將更新。** Amazon銷售渠道使用價格、客戶電子郵件和客戶名稱更新訂單詳細資訊。 在此更新期間，Amazon訂單將建立 [!DNL Commerce] 命令。 的 [!DNL Commerce] 訂單編號顯示，訂單資訊 _[!UICONTROL Orders]_頁籤。 |
| 4 | **建立新客戶帳戶。** 如果按您的訂單設定配置，且客戶不在您的 [!DNL Commerce] 資料庫，在 [!DNL Commerce] 資料庫使用Amazon訂單中相應的客戶資訊。 如果您選擇 `No Customer Creation (guest)` 在您的訂單設定中，順序 [!DNL Commerce] 來賓進程，而不是在資料庫中建立客戶。 現在，如果 [!DNL Commerce] 系統與ERP/OMS/WMS整合，在內部放置和建立的新訂單的整合過程中，系統會拾取訂單 [!DNL Commerce]。 |
| 5 | **訂單已發運。** 從 [!DNL Commerce] 訂單處理頁，您可以發運訂單並添加跟蹤編號。 當所有項都標籤在 `Shipped` 狀態：<ul><li>的狀態 [!DNL Commerce] 訂單更改 `Complete`。</li><li>Amazon銷售渠道訂單的狀態更改為 `Shipped`。</li><li>跟蹤號同步到Amazon,Amazon中訂單的狀態更改為 `Shipped`。</li><li>發運通知通過Amazon發送給客戶，而不是從 [!DNL Commerce] (根據Amazon的政策) |

## 示例：由Amazon履行

| 步驟 | 說明 |
|---|---|
| 1 | **Amazon履行的命令被下達給Amazon。** |
| 2 | **訂單已導入。** 在將訂單分配到 `Shipped` Amazon 由於Amazon擁有此產品的庫存，因此它可防止對您的倉庫/庫存管理造成干擾。 |
| 3 | **訂單詳細資訊將更新。** 如果在 [順序設定](./order-settings.md),Amazon命令將建立 [!DNL Commerce] 建立為狀態為 `Complete`。 |
