---
title: 將清單連結至Walmart
description: '將 [!DNL Commerce] 產品的清單連線到 [!DNL Walmart Marketplace]以開始銷售。'
feature: Sales Channels, Integration, Products, Tools and External Services
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: 8a1f95cdb8817cfcc6ffa96b584c66e680a1c282
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 0%

---

# 將清單連結至Walmart

如同其他市集，[!DNL Walmart]可讓協力廠商賣家列出其他人所銷售的專案。

- [!DNL Walmart Marketplace]使用產品識別碼（例如UPC和GTIN）來比對產品與現有[!DNL Walmart Marketplace]清單。

- 對於相符的產品，Walmart Marketplace會列出更新專案，在您從[!DNL Channel Manager]連線產品時包含[!DNL Commerce]產品優惠。

- 通常，具有最低價格的產品優惠方案會先出現在[!DNL Walmart Marketplace]清單中，但其他因素（如評論）也會影響刊登版位。

## 比對產品

當您符合產品時，管道管理員會將產品資料傳送至[!DNL Walmart Marketplace]，以搜尋具有符合對應[!DNL Commerce]產品屬性的屬性值之現有清單。 相符條件是由您商店管道的[屬性對應組態](map-catalog-attributes.md)所決定。

如果找到相符專案，現有產品清單會更新以新增您的選件。

### 必要條件

比對產品之前，請先確認產品目錄屬性值符合Walmart要求，並設定產品屬性設定。 請參閱[對應目錄屬性](map-catalog-attributes.md)。

#### 選取並比對產品

1. 開啟連線的銷售管道。

1. 從&#x200B;**[!UICONTROL Listings]**&#x200B;中，選取要比對且處於&#x200B;*[!UICONTROL Draft]*&#x200B;狀態的產品。

   ![從清單中選取產品，並傳送以符合](assets/products-in-marketplace-sales-channel.png){width="500" zoomable="yes"}

1. 選取&#x200B;**[!UICONTROL Match Products]**。

   訊息會指出為了比對而傳送的產品數量。

   在比對作業完成之前，所選取產品的狀態會變更為&#x200B;[!UICONTROL *處理中*]。 Walmart Marketplace最多可能需要30分鐘才能完成配對作業。

### 檢查比對狀態

比對完成後，請選取&#x200B;**[!UICONTROL Refresh products]**&#x200B;以檢視目前的產品狀態。 *符合*&#x200B;或&#x200B;*錯誤*。

- **[!UICONTROL Match]**&#x200B;表示產品已成功比對。 您的產品選件已連線至現有的沃爾瑪市集清單。 如果[市集存放區不在作用中](walmart-requirements.md#walmart-marketplace-store-status)，則&#x200B;*[!UICONTROL Staged for Match]*&#x200B;會顯示在&#x200B;*[!UICONTROL Status detail]*&#x200B;欄中。 啟動[!DNL Walmart Marketplace]存放區時，會自動連線階段產品。

- **[!UICONTROL Error]**&#x200B;指出比對作業因下列其中一個問題而失敗：

   - 由於連線問題，[!DNL Channel Manager]無法傳送以進行比對。

   - 找不到相符專案。

   - 找到相符專案，但清單無法連線，因為[!DNL Walmart Marketplace]傳回錯誤碼。 請參閱&#x200B;**[!UICONTROL Error Description]**&#x200B;以取得問題的相關資訊。

### 檢視沃爾瑪的清單

比對產品後，請檢閱更新的產品清單，並從[[!UICONTROL Walmart Marketplace Seller Account Items]儀表板](https://seller.walmart.com/items-and-inventory/manage-items)驗證產品詳細資料、價格和存貨數量，以檢閱更新的產品。

### 產品比對錯誤疑難排解

如果產品比對作業失敗並出現錯誤，則錯誤訊息會顯示在[!UICONTROL Channel Manager]產品清單的&#x200B;*[!UICONTROL Status detail]*&#x200B;欄中。

傳回的常見錯誤為產品ID值的格式不正確或缺少必要屬性。

#### 修正產品ID值

| 型別 | 說明 | 範例 |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12,12位數的數字，包含檢查位數。 </br></br>如果您的UPC少於12位數，例如UPC-E是8位數，請加入結尾的零以符合要求。 | 從`45678912345`變更為`045678912345` |
| GTIN | GTIN-14,14位數的數字，包含核取數字。 </br></br>如果您的GTIN少於14位數，請新增前導零</br>以符合要求。 | 將`456789123456`變更為`0045678912345` |
| EAN | GTIN-13,13位數的數字，包含檢查位數。 </br></br>如果您的EAN少於13位數，請新增前置的</br>個零以符合要求。 | 從`4567891234`變更為`0004567891234` |

如需Walmart Marketplace錯誤碼的詳細資訊，請參閱[Walmart賣家說明](https://sellerhelp.walmart.com/s/guide?article=000005844)。

## 上傳新產品清單

對於在Walmart Marketplace上沒有相符項的產品，請使用Walmart產品類別Excel範本大量上傳產品清單。 您會使用從您的[!DNL Commerce]執行個體匯出的產品目錄資料來填入Walmart範本。

對於新產品清單，請檢查您的產品目錄，以確保您計畫在Walmart Marketplace上銷售的產品具有Walmart Marketplace產品清單所需的屬性。

**Walmart Marketplace清單 — 屬性需求**

| **屬性** | **需求層級** |
|--------------------------|-----------------------|
| SKU | 必填 |
| 產品名稱 | 必填 |
| 產品ID型別 | 必填 |
| 產品ID | 必填 |
| 品牌 | 必填 |
| 簡短說明 | 必填 |
| 售價 | 必填 |
| 網站說明 | 必填 |
| 主要影像URL | 必填 |
| 送貨重量 | 必填 |
| 主要功能 | 建議 |
| 型號 | 建議 |
| 製造商名稱 | 建議 |
| 製造商零件編號 | 建議 |
| 大小 | 建議 |
| 顏色 | 建議 |
| 主要影像URL | 可選 |
| 其他影像URL | 可選 |
| 製造商 | 可選 |

### 必要條件

- 確認您符合[沃爾瑪需求](walmart-requirements.md)。

- 在您的[!DNL Commerce]產品目錄中，確認要列在Walmart Marketplace的產品目錄設定具有所有必要的屬性，並符合Walmart Marketplace內容准則。

- 確認cron工作正在執行中，以完成匯出作業。

   - 若為內部部署執行個體，請參閱[設定並執行cron](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/cli/configure-cron-jobs.html)。

   - 若為Adobe雲端基礎結構，請參閱[設定cron工作](https://experienceleague.adobe.com/docs/commerce-cloud-service/user-guide/configure/app/properties/crons-property.html)。

### 建立要上傳的產品資料檔案

1. 從您的[Walmart賣家帳戶](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller)，從Walmart賣家中心下載產品清單範本。

   - 從產品目錄專案頁面中，選取&#x200B;**[!UICONTROL Add Items]**。 然後，選取&#x200B;**[!UICONTROL Add items in bulk]**。

     ![在Walmart Marketplace專案組態中大量新增專案](assets/walmart-seller-account-add-items-bulk.png){width="600" zoomable="yes"}

   - 在下載頁面上，選取&#x200B;**[!UICONTROL Full Setup]**。 然後，選取專案類別並下載類別範本。

     在Walmart Marketplace專案組態中![下載類別範本選項](assets/walmart-seller-account-full-setup-download.png){width="600" zoomable="yes"}

   - 確認範本包含產品清單的必要和建議屬性。

1. 從[!DNL Commerce] Admin中，選取要從您的Adobe[!DNL Commerce]網站匯出的產品資料。

   - 從管理員中，選取&#x200B;[!UICONTROL **系統** >資料傳輸> **匯出**]。

   - 在[!UICONTROL Entity Type]欄位的[!UICONTROL Export]頁面上，選取&#x200B;[!UICONTROL **產品**]。

   - 在[!UICONTROL Entity Attributes]表格中，設定產品資料匯出的選取條件。

     使用篩選器來選取和設定套用至您銷售的產品類別的屬性值。 請務必加入沃爾瑪的必要和建議屬性。 (如需詳細指示，請參閱Adobe[!DNL Commerce]使用手冊中的[匯出資料](https://experienceleague.adobe.com/docs/commerce-admin/systems/data-transfer/data-export.html)。)

     若要在匯出中省略屬性，請選取該列開頭的&#x200B;[!UICONTROL **排除**]&#x200B;核取方塊。

1. 捲動至屬性表格的結尾，並選取&#x200B;[!UICONTROL **繼續**]&#x200B;以開始資料匯出。

   CSV匯出檔案是使用cron工作透過訊息佇列處理，並儲存在`var/export/folder`中。 （請參閱&#x200B;*設定指南*&#x200B;中的[管理訊息佇列](https://experienceleague.adobe.com/docs/commerce-operations/configuration-guide/message-queues/manage-message-queues.html)。）

1. 開啟Walmart Marketplace產品類別的Excel範本，並使用Excel巨集功能將匯出的產品資料合併至Excel範本。

1. 上傳含有已匯出產品資料的Excel檔案。

   - 返回[Walmart賣家中心](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller)的[產品目錄專案]頁面。

   - 選取&#x200B;[!UICONTROL **新增專案** > **大量新增專案**]。
   - 將完成的試算表拖曳至「上傳」區段。
   - 選取&#x200B;[!UICONTROL **提交**]。
   - 選取&#x200B;[!UICONTROL  **活動摘要**]&#x200B;以檢視進度。

如需完整的指示，請參閱&#x200B;[!DNL *Walmart賣家說明*]&#x200B;中的[使用完整專案規格](https://sellerhelp.walmart.com/s/guide?article=000007680)大量新增專案。
