---
title: Amazon完成工作流程
description: 從Amazon清單完成訂單會遵循從訂單提交到發運的特定順序。
exl-id: 30dd9f97-9193-4c98-bded-e5d8d35b0d05
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 2%

---

# Amazon完成工作流程

## 範例：由商戶履行

| 步驟 | 說明 |
|----|----|
| 1 | **商戶履行的訂單會在Amazon上下。** Amazon會指派狀態 `Pending` 直到驗證客戶的信用卡資訊。 訂購 `Pending` 狀態會自動匯入至Amazon銷售管道，但不會顯示在 _[!UICONTROL Orders]_標籤。 |
| 2 | **訂單經Amazon驗證。** 驗證後，Amazon會將狀態變更為 `Unshipped`. 此狀態變更後，訂單會在Amazon銷售管道中更新，並顯示在 _[!UICONTROL Orders]_標籤。 |
| 3 | **訂單詳細資訊會更新。** Amazon銷售管道會以價格、客戶電子郵件和客戶名稱更新訂單詳細資訊。 在此更新期間，Amazon訂單會建立對應的 [!DNL Commerce] 訂單。 此 [!DNL Commerce] 訂單編號與 _[!UICONTROL Orders]_標籤。 |
| 4 | **已建立新客戶帳戶。** 如果已在您的訂單設定中設定，且您的 [!DNL Commerce] 資料庫，則新客戶會建立在 [!DNL Commerce] 資料庫，使用Amazon訂單中對應的客戶資訊。 如果您選擇 `No Customer Creation (guest)` 在您的訂單設定中，順序會遵循 [!DNL Commerce] 來賓進程，而不是在資料庫中建立客戶。 此時，如果您的 [!DNL Commerce] 系統與ERP/OMS/WMS整合，根據在內部放置和建立的新訂單的整合來提取訂單 [!DNL Commerce]. |
| 5 | **訂單已發運。** 從 [!DNL Commerce] 訂單處理頁面中，您會發運訂單並新增追蹤編號。 所有項目都標示於 `Shipped` 狀態：<ul><li>的狀態 [!DNL Commerce] 訂購變更 `Complete`.</li><li>Amazon銷售管道訂單的狀態變更為 `Shipped`.</li><li>追蹤號碼會同步至Amazon，而Amazon中的順序狀態會變更為 `Shipped`.</li><li>運送通知會透過Amazon(而非 [!DNL Commerce] (根據Amazon的政策)。 |

## 範例：由Amazon(FBA)履行

| 步驟 | 說明 |
|---|---|
| 1 | **Amazon履行的訂單會在Amazon上下。** |
| 2 | **訂單已匯入。** 在將訂單指派至 `Shipped` 狀態(按Amazon)。 由於Amazon有此產品的庫存，因此可防止干擾您的倉庫/庫存管理。 |
| 3 | **訂單詳細資訊會更新。** 若已在 [順序設定](./order-settings.md),Amazon順序會建立對應 [!DNL Commerce] 訂單，並以狀態為 `Complete`. |
