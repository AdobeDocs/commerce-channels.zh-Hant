---
title: 『[!DNL Amazon Sales Channel] 版本注意事項
description: 檢閱發行說明以瞭解全部資訊 [!DNL Amazon Sales Channel] 發行版本。
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2024'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel] 發行說明

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] 可安裝在雲端基礎結構2.3.x和2.4.x版上具有Magento Open Source、Adobe Commerce和Adobe Commerce的執行個體上。Adobe Commerce 2.1、Magento Open Source2.2或Magento1不再支援此擴充功能。
> <br>支援適用於 [!DNL Amazon sales channel]  版本4.0.0和4.1.0 (僅適用於Adobe Commerce 2.3.x版本)。
> <br>[!DNL Amazon sales channel] 版本4.2.0+與Adobe Commerce 2.3.x版本相容，但僅支援Adobe Commerce 2.4.x版本。
>

以下版本說明說明的初始版本 [!DNL Amazon sales channel] 並包含：

![新增](../assets/new.svg) 新功能
![已修正的問題](../assets/fix.svg) 修正和改良
![已知問題](../assets/bug.svg) 已知問題

另請參閱 [即將發行的版本](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) 版本設定、支援和相容性。

另請參閱 [產品可用性](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) 以瞭解哪些Adobe Commerce版本支援此擴充功能。

## v4.5.0

*2023年8月30日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) 新增Adobe.IO API閘道（從MAGI變更），以提升驗證安全性。 `ServicesId` 提供新的UI來管理您的Adobe.IO憑證，類似於其他 [Adobe Commerce服務](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html).

>[!NOTE]
>
>商戶必須確保 [私人和公開API金鑰](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html) 已針對生產環境更新。


![已修正的問題](../assets/fix.svg) 已識別組態設定問題並修正訂單建立流程。

## v4.4.4

*2023年3月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![已修正的問題](../assets/fix.svg) 新增對Adobe Commerce 2.4.6和PHP 8.2的支援。

![已修正的問題](../assets/fix.svg) 減少記錄檔中的雜訊。

![已修正的問題](../assets/fix.svg) 改善提取更新的穩定性。

![已修正的問題](../assets/fix.svg) 簡化執行單一動作（例如提取）或從CLI套用的程式。

![已修正的問題](../assets/fix.svg) 已升級的相依性 `magento/services-connector`.

![已修正的問題](../assets/fix.svg) 修正含有無效國碼之英國帳戶的同步問題。

![已修正的問題](../assets/fix.svg) 以硬式編碼撰寫型錄產品實體的entity_type_id會導致「Magento價格來源」發生問題。

![已修正的問題](../assets/fix.svg) 修正從其他執行個體後端刪除的帳戶無法從UI中刪除的問題。

![已修正的問題](../assets/fix.svg) 修正部分購物車規則中斷訂單匯入的問題。

## v4.4.3

*2023年3月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) 新增對Adobe Commerce 2.4.4的支援。

## v4.4.2

*2021年11月11日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) 更新相依性以支援其他更新的擴充功能。
![修正](../assets/fix.svg) 新增對PHP 8.1的支援。

## v4.4.1

*2021年11月11日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) 已變更Adobe Commerce接收 _使用者名稱_ Amazon中的欄位。 之前，建立訂單時會發生錯誤，因為 _使用者名稱_ 欄位包含特殊字元。 Adobe Commerce現在會收到 _使用者名稱_ 資料並篩選掉特殊字元，以便成功建立訂單。

## v4.4.0

*2021年4月9日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) 為設定新增唯讀模式支援。 另請參閱 [sales channel設定](sales-channel-settings.md).

![修正](../assets/fix.svg) 已變更資料流程，以便相同執行個體的多個副本可同時擷取更新。

![修正](../assets/fix.svg) 已變更同步處理帳戶資訊的同步處理程式。 新增cron作業以與遠端帳戶同步，並在CLI命令中新增相同的功能。

![修正](../assets/fix.svg) 新增CLI命令引數和標幟，以更精確控制。

![修正](../assets/fix.svg) 已修正系統組態中的背景工作(cron)來源。

![修正](../assets/fix.svg) 修正國家代碼設為波多黎各(PR)時無法建立訂單的問題。

## v4.3.0

*2021年3月3日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) <!--CHAN-xxxx-->此 _訂單詳細資料_ 功能已重新設計，不再依賴 _匯入訂單_ 設定。 現在，所有訂單的訂單詳細資料都會顯示在AmazonSales Channel介面中。

![修正](../assets/fix.svg) 在 _[!UICONTROL Marketing]_功能表，名稱已變更：_[!UICONTROL Amazon]_ 至 _[!UICONTROL Amazon Sales Channel]_.

![已知問題](../assets/bug.svg) **重要**：Adobe Commerce 2.4.0相容性的已知問題已在Adobe Commerce 2.4.1版本中解決。

- 中的Amazon cron程式 `error` state
- 在資料庫中建立存放區時，使用Commerce 2.4.0進行安裝失敗
- 安裝MSI時，建立產品失敗

## v4.2.0

*2021年3月3日*

[!BADGE 支援]{type=Informative tooltip="支援"}

如果您有前一個 [!DNL Amazon sales channel] 已安裝版本，並嘗試將Adobe Commerce更新至2.4.0版，系統會提示您更新擴充功能，然後才能完成Adobe Commerce更新。

![已知問題](../assets/bug.svg) 時間 [!DNL Amazon sales channel] 4.2.0已與2.4.0版整合，而且 [Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en) 已啟用，有一個已知問題阻止在您的Commerce目錄中新增產品。 此問題將在未來的Commerce版本中解決。

![新增](../assets/new.svg) [!DNL Amazon sales channel] 已增強以接受文字型位址資料，並將其比對至標準化的位址格式，包括城市、州和郵遞區號。 此更新可讓訂單和運送資料與Amazon同步（同步），而不會出現地址錯誤。<br/>例如，購物者輸入城市、州/省、郵遞區號如下 `Escondido, californiA 92025-1501`. AmazonSales Channel會匯入資料並將資料與標準格式配對，如 `Escondido, CA 92025`，然後以這個標準化格式將其同步回Amazon。

![新增](../assets/new.svg) 新增對PHP 7.4的支援。

![新增](../assets/new.svg) <!--CHAN-4334-->新增對Adobe Commerce 2.4.x的支援。舊版可能與Commerce 2.4.x相容，但不受支援。 另請參閱 [即將發行的版本](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html) 版本相容性。 必須先將AmazonSales Channel更新至4.2.0，才能完成Adobe Commerce 2.4.0更新。

![修正](../assets/fix.svg) <!--CHAN-4431-->已修正導致 _存取遭拒_ 英國客戶的錯誤。

![修正](../assets/fix.svg) <!--CHAN-4394-->修正導致Amazon送貨狀態無法同步至相應Commerce訂單的問題，因此「鎖定」訂單的送貨狀態為 `Pending` 在Commerce和 `Unshipped` 在Amazon中。 透過新的標準化地址功能，這些送貨狀態錯誤已解決。

![修正](../assets/fix.svg) <!--ticket#-->更新訂單同步（同步）以忽略失敗的訂單匯入，從而減少多次同步嘗試並允許後續匯入進行處理，每五分鐘提交一次訂單同步請求。 同步錯誤仍記錄在錯誤記錄中，但標籤為「已處理」以允許進一步的記錄功能。 另外， [!DNL Amazon sales channel] 現在會自動移除針對無法在Commerce中建立的訂單收集的多餘資料。

![修正](../assets/fix.svg) 已更新錯誤記錄，以收集未攔截到例外和擴充功能更新錯誤的詳細資訊。

![修正](../assets/fix.svg) <!--ticket#-->修正造成初次同步處理的問題 _最低價格_ 資料因遺失而失敗 _價格_ 值。

![修正](../assets/fix.svg) <!--CHAN-4410-->已修正導致中過濾錯誤的問題 _Amazon訂單_ 日期範圍欄位留空時進行檢視。

![修正](../assets/fix.svg) <!--CHAN-4439-->修正導致數量相關庫存與履行同步錯誤的問題。 現在，擴充功能會先向下舍入以小數輸入的數量值，再與Amazon同步。<br/> 例如，當商家手動輸入 `2.5`，擴充功能會將值向下舍入為 `2` 然後與Amazon同步更新的數量。

## v4.1.0

*2020年5月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) <!--4247, 4230-->已變更訂單匯入程式，以符合Commerce訂單要求。 這些變更修正了Commerce無法為匯入訂單建立對應訂單的問題。 另請參閱 [管理訂單](managing-orders.md) 以取得訂單封鎖程式和解決方案的相關資訊。

![新增](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->已更新 _最近的訂單_ 區段並新增一個 _所有訂單_ 此檢視畫面會顯示您所有的Amazon訂單，包括篩選選項和用於檢視更多訂單的分頁。 另請參閱 [Amazon商店控制面板](amazon-store-dashboard.md) 和 [檢視Amazon訂單](amazon-orders-all.md).

![新增](../assets/new.svg) 已新增 _[!UICONTROL Order Notes]_重新設計的欄_[!UICONTROL Amazon Orders]_ 表格（兩者） _[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_ 檢視。 _[!UICONTROL Order Notes]_告知商家訂單的匯入發生問題。 另請參閱 [檢視Amazon訂單](amazon-orders-all.md).

![新增](../assets/new.svg) <!--CHAN-4013-->更新產品條件引數以符合 [Amazon已續約](https://sell.amazon.com/programs/renewed) 程式。 另請參閱 [已續訂的產品](renewed-products.md).

![新增](../assets/new.svg) <!--CHAN-3680-->已更新 [Amazon訂單詳細資料](amazon-order-details.md) 針對Amazon履行的訂單加入「一般資料」。 另請參閱 [履行者](fulfilled-by.md).

![修正](../assets/fix.svg) <!--CHAN-4069-->修正導致商店卡上圖示扭曲的問題。

![修正](../assets/fix.svg) <!--CHAN-4165-->已更正錯誤，防止 _登入_ 畫面會在工作階段逾時之後顯示。

![修正](../assets/fix.svg) <!--CHAN-4211-->已修正導致Amazon訂單稅額無法匯入新Commerce訂單的問題。

![修正](../assets/fix.svg) <!--CHAN-4234-->修正導致商店控制面板上顯示的收入總計包含訂單的問題 `Canceled` 或 `Error` 狀態。

![修正](../assets/fix.svg) <!--CHAN-4326-->修正造成訂單匯入錯誤，且與使用的協力廠商擴充功能相關的問題 _Magento Shipping_ 建立訂單的方法。

![修正](../assets/fix.svg) <!--CHAN-4357-->已修正執行cron同步時導致錯誤的問題。 CLI命令已新增鎖定，可防止兩個cron作業同時同步。

![修正](../assets/fix.svg) 已更新內容安全性原則，以支援Commerce 2.3.5版。

## v4.0.0

*2020年3月25日*

[!BADGE 支援]{type=Informative tooltip="支援"}

>[!IMPORTANT]
>
>Amazon 2.3.5不支援Adobe CommerceSales Channel4.0.0。如需Adobe Commerce 2.3.5的支援，請升級至AmazonSales Channel4.1.0。

![新增](../assets/new.svg) 推出新的 [AmazonSales Channel](amazon-sales-channel-home.md) 首頁，改善商店資訊的「卡片檢視」。

![新增](../assets/new.svg) 推出新的 [存放區儀表板](amazon-store-dashboard.md) 包含清單、最近訂購和商店設定資訊。

![新增](../assets/new.svg) 推出更簡單、更精簡的 [上線流程](amazon-onboarding-home.md) 和 [預設商店設定](default-store-settings.md) 讓您的商店更快整合。

![已知問題](../assets/bug.svg) <!--CHAN-4102--> 時間 [建立屬性](managing-attributes.md) 用於從清單和匯入影像 **存放區檢視** 設為 `All Store Views (Global)`，一個已知問題存在，無法將影像匯入至所有存放區檢視。 如果您變更的設定 **儲存檢視（將值匯入）** 影像會匯入至特定存放區。

## v3.0.1

*2019年11月11日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) **數值欄位設定**： <!--CHAN-3779-->需要數值的欄位已更新為僅接受數值字元。 範例：訂價規則設定>調整金額欄位

![修正](../assets/fix.svg) **使用手冊連結**： <!--CHAN-3778-->不正確 _使用手冊_ 已更正連結。

![修正](../assets/fix.svg) **複製Amazon清單**： <!--CHAN-3593-->先前報告導致重複Amazon清單的問題現在已得到更正。 在此版本之前，擴充功能在匯入清單時，已將Amazon地區的國家/地區代碼新增至SKU值。 此清單與型錄專案相符，但擴充功能建立了包含附加SKU的新重複清單。 在此版本中，擴充功能不會修改匯入清單的SKU，且不會變更現有清單。 您可以使用 [!UICONTROL End Listing(s)] 用於移除重複清單的「在Amazon上」選項。

## v3.0.0

*2019年十月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) **Amazon UK Marketplace現已推出**：使用者在建立和整合Commerce商店時，可選擇英國的Marketplace。 此英國升級包含下列專案的額外支援：

- [Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [產品稅捐代碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} 資訊。

![新增](../assets/new.svg) **改善的記錄**： <!--CHAN-3642, 3672-->已實作 **啟用偵錯記錄** 功能，可在需要疑難排解時收集其他同步資料。 請參閱 [Sales Channel設定](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html) 組態參考中的主題。

![修正](../assets/fix.svg) **產品目錄**： <!--CHAN-3687-->修正無法將具有Amazon清單之匯入的影像套用至對應Commerce目錄產品的問題。

![修正](../assets/fix.svg) **訂單建立**： <!--CHAN-3708-->已修正導致Commerce無法為不符合Commerce目錄產品的Amazon訂單建立訂單的問題。

![已知問題](../assets/bug.svg) **複製Amazon清單**： <!--CHAN-3593-->此問題會導致目錄使用相同的SKU為匯入清單建立專案，但會在結尾新增地區代碼。 Amazon接著會將修改過的SKU處理為新專案，並建立清單。 此問題將在未來版本中解決。

## v2.0.0

[!BADGE 支援]{type=Informative tooltip="支援"}

>[!NOTE]
>
>1.0.0版僅在限量版中提供。

![新增](../assets/new.svg)  **簡化的入門與維護**：透過管理員提供的詳細指示，透過逐步流程新增並整合您的Amazon賣家帳戶。 透過單一儀表板維護您的商店、帳戶和列出的產品。

![新增](../assets/new.svg)  **多帳戶支援**：透過管理員管理及監控多個Amazon品牌和Marketplace地區。

![新增](../assets/new.svg)  **智慧型定價**：設定自動重新訂價規則，增加您獲得夢寐以求的Buy Box的機會。 設定價格，以動態調整至目前的Buy Box價格，或最低競爭者價格。 設定重新訂價的上限以保護您的利潤。

![新增](../assets/new.svg)  **清單管理**：自動化產品清單，並使用清單規則將您的商務目錄同步至Amazon Marketplace。 新增特定覆寫，以精細控制您的方案。 直接從「管理員」監視及管理所有清單。

![新增](../assets/new.svg)  **一致的Inventory management**：保持您的Commerce和Amazon庫存數量不間斷的同步。

![新增](../assets/new.svg)  **訂單與履行管理**：透過控制面板追蹤Amazon訂單，並順暢通訊和更新存貨。 完成並追蹤由Amazon、已履行的商家或多種方法所履行的訂單出貨。

![已知問題](../assets/bug.svg)  更新產品數量的等待時間可能會更長。 產品數量的更新可能需要約兩個小時才能同步。

![已知問題](../assets/bug.svg)  匯入的訂單可能具有 _Prime_ 或 _Premium_ 訂購。 您應在Amazon賣家帳戶中驗證這些訂單。

![已知問題](../assets/bug.svg)  不符合資格的套件產品可能會顯示為「符合在Amazon上列出的資格」。 套件產品中的其中一種產品可能不符合條件。 如果您遇到問題，請檢查套裝產品專案的適用狀態。

![已知問題](../assets/bug.svg)  使用Inventory management for Commerce 2.3.x時，建立訂單時可能不會觸發部分股票重新索引。 可銷售數量會每小時重新計算，這可能會導致在此更新間隔期間過度銷售。
