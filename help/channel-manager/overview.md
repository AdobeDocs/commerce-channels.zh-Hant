---
title: '''簡介 [!DNL Channel Manager]『'
description: '''瞭解如何安裝和使用 [!DNL Channel Manager] 將Adobe Commerce和Magento Open Source商店與Walmart Marketplace整合，並建立銷售管道，以便從您的Commerce管理員順暢地管理市集清單、定價、存貨和銷售。'
role: Leader, Admin, User
level: Intermediate
exl-id: 91265973-d2ad-4925-aa10-260d7e186f20
source-git-commit: 850aece134084e108b324a964d7d834042c7ddfd
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# 簡介 [!DNL Channel Manager]

[!DNL Channel Manager] 透過整合Adobe Commerce或Magento Open Source產品目錄與 [!DNL Walmart Marketplace].

![[!DNL Channel Manager] 擴充功能管理員檢視](assets/channel-manager-home.png){width="700" zoomable="yes"}

[!DNL Channel Manager] 支援想要銷售的Adobe Commerce或Magento Open Source商家 [!DNL Walmart Marketplace] 藉由擴充 [!DNL Commerce] 管理員。 替換為 [!DNL Channel Manager] 已安裝、商店管理員與營運人員可管理 [!DNL Walmart Marketplace] Commerce環境中的銷售、庫存和產品定價無懈可擊。

擴充的「管理員」可簡化作業，因為商戶可使用相同的工作流程與處理，管理來自兩者的銷售 [!DNL Commerce] 店面和沃爾瑪市集。

安裝及設定之後 [!DNL Channel Manager]，您可以使用下列功能來管理Walmart Marketplace的銷售訂單：

* **清單管理** — 輕鬆連線產品清單，比對產品來自 [!DNL Commerce] 目錄至現有 [!DNL Walmart Marketplace] 清單。

* **Inventory management** — 商戶的Marketplace賣家帳戶中的專案會自動同步並更新，從 [!DNL Commerce] 以確儲存貨層次準確。

* **價格更新** — 透過自動價格同步化來維持市集清單的精確定價。 當Adobe Commerce中的價格變更時，這些變更會反映在Marketplace中。

* **Order management** — 在市集內建立新訂單時， [!DNL Channel Manager] 會與Adobe Commerce同步訂單，並將訂單確認傳送至marketplace。 此確認會確保為每筆訂單預留存貨。 最後一個步驟是建立以下檔案中的對應訂單： [!DNL Commerce] 處理訂單管理系統。

* **送貨管理** — 當訂單在Adobe Commerce中標示為已出貨時，出貨更新會傳送至 [!DNL Walmart Marketplace]. 此通知可確保賣方符合其履行SLA要求，並且客戶會收到其目前訂單的送貨更新通知。

* **取消** — 在Adobe Commerce中取消訂單時， [!DNL Channel Manager] 會將更新的訂單資訊傳送至市集，以復寫對應市集訂單的動作。 訂單取消完成後， [!DNL Commerce] 存貨數量更新以反映退回的料號，而存貨更新會自動同步至 [!DNL Walmart Marketplace].

* **退貨與退款** — 當沃爾瑪市集要求退貨透過Adobe Commerce或Magento Open Source銷售管道訂購的商品， [!DNL Channel Manager] 傳送傳回要求資訊至Commerce銷售管道存放區以復寫傳回要求。 然後，您可以使用來處理退款 [!DNL Commerce] [退款工作流程](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/order-management/credit-memos/credit-memos.html#refund-workflow)，離線方法。 退款完成之後， [!DNL Channel Manager] 將更新同步至Walmart，以便可以更新市集賣家帳戶中的退貨狀態以反映退款。

## 的預期延遲 [!DNL Channel Manager] 操作

資料同步程式會在 [!DNL Channel Manager] 和一個已連結 [!DNL Walmart Marketplace] 存放區需要一些時間才能完成。 檢閱的預期處理時間 [!DNL Channel Manager] 作業，協助規劃銷售通路作業。

**預估延遲： [!DNL Channel Manager] 操作**

| **作業** | **說明** | **預期延遲** |
|------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|
| 將產品新增至 [!DNL Channel Manager] | 從中選擇產品 [!DNL Commerce] 產品目錄並將其匯入 [!DNL Channel Manager]. | **最多五分鐘** — 如果您選取許多產品（例如，整個產品目錄），則匯入程式會花費較長的時間。 |
| 比對產品於 [!DNL Walmart Marketplace] | 選取產品清單于 [!DNL Channel Manager] 並傳送給沃爾瑪進行比對。 | **長達30分鐘** — 如果您選取許多產品，則相符程式會花費較長的時間（視選取的數量而定）。 |
| 詳細目錄更新 | 當Commerce中的存貨數量變更時， [!DNL Channel Manager] 將更新同步至Walmart。 | **最多10分鐘** |
| 價格更新 | 當產品價格變更時， [!DNL Channel Manager] 將更新同步至Walmart。 | **最多五分鐘** |
| 從Walmart訂購同步至 [!DNL Commerce] | 客戶訂購 [!DNL Commerce] 沃爾瑪市集上的商品。 Walmart將訂單傳送至 [!DNL Channel Manager]. 訂單會顯示在訂單儀表板中。 | **長達30分鐘** |
| 訂單建立於 [!DNL Commerce] Order Management | [!DNL Channel Manager] 建立 [!DNL Commerce] Walmart訂單的訂單，並更新訂單儀表板，以包含 [!DNL Commerce] 訂單編號。 | **最多五分鐘** |
| 送貨狀態更新於 [!DNL Commerce] Order Management | 當訂單從Commerce出貨時， [!DNL Channel Manager] 更新訂單儀表板中的「出貨」狀態，並將更新傳送至Walmart市集，以便通知客戶。 | **最多五分鐘** |
| Commerce Order Management訂單取消更新 | 從Commerce取消訂單時， [!DNL Channel Manager] 更新訂單儀表板中的訂單狀態，並將更新傳送至Walmart市集，以便通知客戶。 訂單取消完成後， [!DNL Commerce] 庫存數量更新以反映退回的料號。 然後 [!DNL Channel Manager] 將更新同步至 [!DNL Walmart Marketplace]. | **最多五分鐘** |


