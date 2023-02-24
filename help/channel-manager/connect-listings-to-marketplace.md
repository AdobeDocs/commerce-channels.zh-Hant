---
title: 將上市業務連接到沃爾瑪
description: '''連接清單 [!DNL Commerce] 產品 [!DNL Walmart Marketplace]開始賣。'
exl-id: 78078b14-ebdd-415d-9486-66b0150167aa
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '1096'
ht-degree: 0%

---

# 將上市業務連接到沃爾瑪

和其他市場一樣， [!DNL Walmart] 允許第三方銷售者列出由他人銷售的項目。

- [!DNL Walmart Marketplace] 使用產品識別碼（如UPC和GTIN），將產品與現有 [!DNL Walmart Marketplace] 清單。

- 對於匹配的產品，沃爾瑪市場將更新列入 [!DNL Commerce] 產品優惠方案，當您從 [!DNL Channel Manager].

- 通常，價格最低的產品選件會先出現在 [!DNL Walmart Marketplace] 清單，但評論等其他因素也會影響版位。

## 匹配產品

當您符合產品時，管道管理員會將產品資料傳送至 [!DNL Walmart Marketplace] 搜索具有與映射的屬性值的現有清單 [!DNL Commerce] 產品屬性。 符合條件由 [屬性映射配置](map-catalog-attributes.md) 的通道。

如果找到相符項目，則會更新現有的產品清單以新增優惠方案。

### 必要條件

在匹配產品之前，請驗證您的產品目錄屬性值是否滿足Walmart要求，並配置產品屬性設定。 請參閱 [映射目錄屬性](map-catalog-attributes.md).

#### 選取並比對產品

1. 開啟連接的銷售渠道。

1. 從 **[!UICONTROL Listings]**，請選取要比對的產品 *[!UICONTROL Draft]* 狀態。

   ![從清單中選擇產品併發送以進行匹配](assets/products-in-marketplace-sales-channel.png)

1. 選擇 **[!UICONTROL Match Products]**.

   訊息會指出要比對的傳送產品數量。

   所選產品的狀態將更改為 [!UICONTROL *處理*] 直到匹配操作完成。 沃爾瑪市場完成比賽操作可能需要30分鐘。

### 檢查匹配狀態

比對完成後，選取 **[!UICONTROL Refresh products]** 查看當前產品狀態。 *符合* 或 *錯誤*.

- **[!UICONTROL Match]** 表示產品已成功匹配。 你的產品報價與沃爾瑪Marketplace的一份上市交易有關。 若 [市場商店不活動](walmart-requirements.md#walmart-marketplace-store-status), *[!UICONTROL Staged for Match]* 會顯示在 *[!UICONTROL Status detail]* 欄。 當 [!DNL Walmart Marketplace] 儲存已啟用。

- **[!UICONTROL Error]** 表示匹配操作由於以下問題之一而失敗：

   - [!DNL Channel Manager] 由於連線問題，無法傳送以進行比對。

   - 未找到匹配項。

   - 找到匹配項，但無法連接清單，因為 [!DNL Walmart Marketplace] 傳回錯誤碼。 請參閱 **[!UICONTROL Error Description]** 以取得問題的相關資訊。

### 查看沃爾瑪上市情況

匹配產品後，複查更新的產品清單，並驗證產品詳細資訊、價格和庫存數量， [[!UICONTROL Walmart Marketplace Seller Account Items] 儀表板](https://seller.walmart.com/items-and-inventory/manage-items) 檢閱更新的產品。

### 疑難排解產品比對錯誤

如果產品比對作業失敗並出現錯誤，錯誤訊息會顯示在 *[!UICONTROL Status detail]* 欄中 [!UICONTROL Channel Manager] 產品清單。

傳回的常見錯誤是格式錯誤的產品ID值或缺少必要屬性。

#### 修正產品ID值

| 類型 | 說明 | 範例 |
|------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|
| UPC | GTIN-12,12位數字，包括支票數字。 </br></br>如果UPC的位數少於12位數（如8位數的UPC-E），請添加結尾零以滿足要求。 | 變更自 `45678912345` to `045678912345` |
| GTIN | GTIN-14,14位數字，包括支票數字。 </br></br>如果GTIN的位數少於14位數，請加上前導零 </br>才能滿足要求。 | 變更 `456789123456` to `0045678912345` |
| EAN | GTIN-13,13位數字，包括支票數字。 </br></br>如果EAN的位數少於13位，請添加行距 </br>零以滿足要求。 | 變更自 `4567891234` to `0004567891234` |

有關Walmart Marketplace錯誤代碼的詳細資訊，請參閱 [沃爾瑪賣家幫助](https://sellerhelp.walmart.com/s/guide?article=000005844).

## 上傳新產品清單

對於在Walmart Marketplace上沒有匹配的產品，使用Walmart產品類別Excel模板批量上載產品清單。 您使用從您的 [!DNL Commerce] 例項。

對於新產品清單，請檢查您的產品目錄，以確保您計畫在沃爾瑪市場銷售的產品具有沃爾瑪市場產品清單所需的屬性。

**Walmart Marketplace清單 — 屬性要求**

| **屬性** | **需求層** |
|--------------------------|-----------------------|
| SKU | 必填 |
| 產品名稱 | 必填 |
| 產品ID類型 | 必填 |
| 產品ID | 必填 |
| 品牌 | 必填 |
| 簡短說明 | 必填 |
| 售價 | 必填 |
| 網站說明 | 必填 |
| 主影像URL | 必填 |
| 裝運重量 | 必填 |
| 主要功能 | 建議 |
| 型號 | 建議 |
| 製造商名稱 | 建議 |
| 製造商部件號 | 建議 |
| 大小 | 建議 |
| 顏色 | 建議 |
| 主影像URL | 可選 |
| 其他影像URL | 可選 |
| 製造商 | 可選 |

### 必要條件

- 確認您符合 [沃爾瑪要求](walmart-requirements.md).

- 在 [!DNL Commerce] 產品目錄，驗證要在Walmart Marketplace上列出的產品的目錄配置是否具有所有必需屬性，並符合Walmart Marketplace內容指南。

- 驗證cron作業是否正在運行以完成導出操作。

   - 如需內部部署例項，請參閱 [設定並執行cron](https://devdocs.magento.com/guides/v2.4/config-guide/cli/config-cli-subcommands-cron.html).

   - 有關Adobe雲基礎架構，請參閱 [設定cron作業](https://devdocs.magento.com/cloud/configure/setup-cron-jobs.html).

### 建立要上傳的產品資料檔案

1. 從 [沃爾瑪賣家賬戶](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller)，從沃爾瑪銷售中心下載產品清單模板。

   - 從「產品目錄項目」頁中，選擇 **[!UICONTROL Add Items]**. 然後，選取 **[!UICONTROL Add items in bulk]**.

      ![在Walmart Marketplace項目配置中以批量方式添加項目](assets/walmart-seller-account-add-items-bulk.png)

   - 在下載頁面上，選取 **[!UICONTROL Full Setup]**. 然後，選擇項目類別並下載類別模板。

      ![在Walmart Marketplace項配置中下載類別模板選項](assets/walmart-seller-account-full-setup-download.png)

   - 確認範本包含產品清單的必要和建議屬性。

1. 從 [!DNL Commerce] 管理員，選取要從您的Adobe匯出的產品資料 [!DNL Commerce] 頁簽。

   - 在管理員中，選取 [!UICONTROL **系統** >資料傳輸> **匯出**].

   - 在 [!UICONTROL Export] 頁面 [!UICONTROL Entity Type] 欄位，選擇 [!UICONTROL **產品**].

   - 在 [!UICONTROL Entity Attributes] 表格，配置產品資料導出的選擇標準。
   ![匯出產品資料頁面，位於 [!UICONTROL [!DNL Commerce] Admin]](assets/walmart-seller-account-full-setup-download.png)

   使用篩選器來選取和設定適用於您銷售的產品類別的屬性值。 確保包括沃爾瑪的必需屬性和推薦屬性。 (請參閱 [匯出資料](https://docs.magento.com/user-guide/system/data-export.html) 在Adobe [!DNL Commerce] 使用手冊，以取得詳細指示。)

   若要從匯出中忽略屬性，請選取 [!UICONTROL **排除**] 核取方塊。

1. 滾動到屬性表的末尾並選擇 [!UICONTROL **繼續**] 以開始資料匯出。

   CSV匯出檔案會透過使用cron工作的訊息佇列處理，並儲存在 `var/export/folder`. (請參閱 [管理消息隊列](https://devdocs.magento.com/guides/v2.4/config-guide/mq/manage-message-queues.html) 在 *Commerce開發人員指南*.)

1. 開啟Walmart Marketplace產品類別的Excel模板，並使用Excel宏功能將導出的產品資料合併到Excel模板中。

1. 上傳包含匯出產品資料的Excel檔案。

   - 返回產品目錄項目頁面，位於 [沃爾瑪賣家中心](https://login.account.wal-mart.com/authorize?responseType=code&amp;clientId=66620dfd-1f3f-479b-8b9c-e11f36c5438b&amp;scope=openId&amp;redirectUri=https://seller.walmart.com/resource/login/sso/torbit&amp;nonce=SX17QLMBKR&amp;state=ZBWWNZXXXM&amp;clientType=seller).

   - 選擇 [!UICONTROL **新增項目** > **大量新增項目**].
   - 將完成的試算表拖曳至「上傳」區段。
   - 選擇 [!UICONTROL **提交**].
   - 選取&#x200B;[!UICONTROL  **活動摘要**] 查看進度。

如需完整指示，請參閱 [使用完整項目規格批量添加項目](https://sellerhelp.walmart.com/s/guide?article=000007680) 在 [!DNL *沃爾瑪賣家幫助*].
