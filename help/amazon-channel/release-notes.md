---
title: '[!DNL Amazon Sales Channel] 發行說明'
description: 請參閱發行說明，了解 [!DNL Amazon Sales Channel] 版本。
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: 3b2f60ad2796ee1fdc8808fc0941d76a603b2213
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 發行說明

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] 可在雲端基礎架構2.3.x版和2.4.x版上，安裝於具有Magento Open Source、Adobe Commerce和Adobe Commerce的執行個體。Adobe Commerce 2.1、Magento Open Source2.2或Magento1不再支援擴充功能。
> <br>支援 [!DNL Amazon sales channel]  僅限Adobe Commerce 2.3.x版上的4.0.0和4.1.0版。
> <br>[!DNL Amazon sales channel] 4.2.0+版與Adobe Commerce 2.3.x版相容，但僅Adobe Commerce 2.4.x版提供支援。

以下版本說明的初始版本 [!DNL Amazon sales channel] 包括：

![新增](../assets/new.svg) 新功能
![修正問題](../assets/fix.svg) 修正和改良
![已知問題](../assets/bug.svg) 已知問題

請參閱 [即將發行的版本](https://devdocs.magento.com/release/){target="_blank"} 版本設定、支援和相容性。

## v4.4.4

*2023年3月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修正問題](../assets/fix.svg) 新增對Adobe Commerce 2.4.6和PHP 8.2的支援。

![修正問題](../assets/fix.svg) 減少日誌中的噪音。

![修正問題](../assets/fix.svg) 已改善提取更新的穩定性。

![修正問題](../assets/fix.svg) 簡化了從CLI執行單一動作類提取或套用的程式。

![修正問題](../assets/fix.svg) 升級的 `magento/services-connector`.

![修正問題](../assets/fix.svg) 修正英國帳戶中國家/地區代碼無效的同步問題。

![修正問題](../assets/fix.svg) 以硬式編碼撰寫目錄產品實體的entity_type_id會造成Magento價格來源問題。

![修正問題](../assets/fix.svg) 修正無法從其他執行個體刪除後端帳戶，也無法從UI刪除的問題。

![修正問題](../assets/fix.svg) 修正部分購物車規則違反訂單匯入的問題。

## v4.4.3

*2023年3月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修正](../assets/fix.svg) 新增對Adobe Commerce 2.4.4的支援。

## v4.4.2

*2021年11月11日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修正](../assets/fix.svg) 更新相依性以支援其他更新的擴充功能。
![修正](../assets/fix.svg) 新增對PHP 8.1的支援。

## v4.4.1

*2021年11月11日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修正](../assets/fix.svg) 變更Adobe Commerce接收 _使用者名稱_ 欄位。 之前，在建立訂單期間，當 _使用者名稱_ 欄位包含特殊字元。 Adobe Commerce現在獲得 _使用者名稱_ 資料並篩選掉特殊字元，以便成功建立順序。

## v4.4.0

*2021年4月9日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新增](../assets/new.svg) 在設定中新增唯讀模式支援。 請參閱 [銷售渠道設定](sales-channel-settings.md).

![修正](../assets/fix.svg) 已變更資料流，讓相同例項的多個副本可同時擷取更新。

![修正](../assets/fix.svg) 變更同步帳戶資訊的同步程式。 新增cron工作以與遠端帳戶同步，並在CLI命令中新增相同功能。

![修正](../assets/fix.svg) 添加CLI命令參數和標籤，以更精確地控制。

![修正](../assets/fix.svg) 更正系統配置中的「Background Tasks(cron)Source(後台任務(cron)源)」。

![修正](../assets/fix.svg) 修正當國家/地區代碼設為波多黎各(PR)時無法建立訂單的問題。

## v4.3.0

*2021年3月3日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修正](../assets/fix.svg) <!--CHAN-xxxx-->此 _訂單詳細資訊_ 功能已重新設計，不再依賴 _導入訂單_ 設定。 訂單詳細資料現在會顯示在AmazonSales Channel介面中，用於所有訂單。

![修正](../assets/fix.svg) 在 _[!UICONTROL Marketing]_功能表中，名稱已從_[!UICONTROL Amazon]_ to _[!UICONTROL Amazon Sales Channel]_.

![已知問題](../assets/bug.svg) **重要**:Adobe Commerce 2.4.0相容性的已知問題已在Adobe Commerce 2.4.1版中解決。

- Amazon cron流程 `error` state
- 在資料庫中建立儲存時，使用Commerce 2.4.0安裝會失敗
- 安裝MSI時建立產品失敗

## v4.2.0

*2021年3月3日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

如果您有之前的 [!DNL Amazon sales channel] 版本，並嘗試將Adobe Commerce更新至2.4.0版時，系統會提示您更新擴充功能，然後您才能完成Adobe Commerce更新。

![已知問題](../assets/bug.svg) 當 [!DNL Amazon sales channel] 4.2.0已與2.4.0版和 [Inventory management](https://docs.magento.com/user-guide/catalog/inventory.html) 啟用時，會出現一個已知問題，導致無法在您的商務目錄中新增產品。 此問題將在未來的Commerce版本中解決。

![新增](../assets/new.svg) [!DNL Amazon sales channel] 已增強功能，以接受文字型位址資料，並將其與標準化位址格式（包括城市、州和郵遞區號）相符。 此更新可讓訂單和運送資料與Amazon同步（同步），而不會發生位址錯誤。<br/>例如，購物者將城市、州、郵遞區號輸入為 `Escondido, californiA 92025-1501`. AmazonSales Channel會匯入資料，並將資料比對為標準格式 `Escondido, CA 92025`，然後以此標準化格式將其同步回Amazon。

![新增](../assets/new.svg) 新增對PHP 7.4的支援。

![新增](../assets/new.svg) <!--CHAN-4334-->新增對Adobe Commerce 2.4.x的支援。舊版可能與Commerce 2.4.x相容，但不支援。 請參閱 [即將發行的版本](https://devdocs.magento.com/release/){:target=&quot;_blank&quot;}以取得版本相容性。 AmazonSales Channel必須更新至4.2.0,Adobe Commerce 2.4.0更新才能完成。

![修正](../assets/fix.svg) <!--CHAN-4431-->修正導致 _拒絕訪問_ 錯誤。

![修正](../assets/fix.svg) <!--CHAN-4394-->修正導致Amazon發運狀態無法同步至對應商務訂單的問題，因此將訂單的發運狀態「鎖定」為 `Pending` 在商務和 `Unshipped` 在Amazon。 使用新的標準化地址功能，已解決這些運送狀態錯誤。

![修正](../assets/fix.svg) <!--ticket#-->更新訂單同步（同步）以忽略失敗的訂單導入，從而減少多次同步嘗試並允許後續導入處理，每五分鐘提交一次訂單同步請求。 同步錯誤仍記錄在錯誤記錄中，但標示為「已處理」以允許進一步記錄功能。 此外， [!DNL Amazon sales channel] 現在會自動移除針對無法在商務中建立之訂單所收集的多餘資料。

![修正](../assets/fix.svg) 更新錯誤記錄，以收集未捕獲的例外狀況和擴充功能更新錯誤的詳細資訊。

![修正](../assets/fix.svg) <!--ticket#-->修正導致初始同步 _最低價格_ 資料因遺失而失敗 _價格_ 值。

![修正](../assets/fix.svg) <!--CHAN-4410-->修正導致 _Amazon訂購_ 日期範圍欄位留空時檢視。

![修正](../assets/fix.svg) <!--CHAN-4439-->修正導致與數量相關的庫存和履行同步錯誤的問題。 擴充功能現在會捨入以小數形式輸入的數量值，再與Amazon同步。<br/> 例如，當商家手動輸入 `2.5`，擴充功能會將值捨入為 `2` 然後將更新的數量與Amazon同步。

## v4.1.0

*2020年5月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新增](../assets/new.svg) <!--4247, 4230-->已變更訂單匯入程式，使其符合商務訂單需求。 這些變更會修正商務無法為匯入訂單建立對應訂單的問題。 請參閱 [管理訂單](managing-orders.md) 以取得訂單封鎖程式和解決方案的相關資訊。

![新增](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->更新 _最近訂購_ 區段，並新增 _所有訂單_ 顯示所有Amazon訂單的檢視，包括篩選選項和分頁，以檢視更多訂單。 請參閱 [Amazon商店儀表板](amazon-store-dashboard.md) 和 [檢視Amazon訂單](amazon-orders-all.md).

![新增](../assets/new.svg) 新增 _[!UICONTROL Order Notes]_重新設計的欄_[!UICONTROL Amazon Orders]_ 表格 _[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_ 檢視。 _[!UICONTROL Order Notes]_讓商家知道訂單的進口有問題。 請參閱 [檢視Amazon訂單](amazon-orders-all.md).

![新增](../assets/new.svg) <!--CHAN-4013-->更新產品條件參數以與 [Amazon續約](https://sell.amazon.com/programs/renewed) 程式。 請參閱 [續訂產品](renewed-products.md).

![新增](../assets/new.svg) <!--CHAN-3680-->已更新 [Amazon訂單詳細資料](amazon-order-details.md) 納入Amazon履行之訂單的「一般資料」。 請參閱 [履行者](fulfilled-by.md).

![修正](../assets/fix.svg) <!--CHAN-4069-->修正造成儲存卡上圖示扭曲的問題。

![修正](../assets/fix.svg) <!--CHAN-4165-->修正防止 _登入_ 螢幕無法在工作階段逾時後顯示。

![修正](../assets/fix.svg) <!--CHAN-4211-->修正Amazon訂單稅額無法匯入新商務訂單的問題。

![修正](../assets/fix.svg) <!--CHAN-4234-->修正商店控制面板上顯示的收入總計包含訂單的問題 `Canceled` 或 `Error` 狀態。

![修正](../assets/fix.svg) <!--CHAN-4326-->修正導致訂單匯入錯誤的問題，此錯誤與使用的協力廠商擴充功能相關聯 _Magento Shipping_ 建立訂單的方法。

![修正](../assets/fix.svg) <!--CHAN-4357-->修正執行cron同步時導致錯誤的問題。 已在CLI命令上添加鎖，該鎖阻止兩個cron作業同時同步。

![修正](../assets/fix.svg) 更新內容安全性原則，以支援Commerce 2.3.5版。

## v4.0.0

*2020年3月25日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

>[!IMPORTANT]
>
>Adobe Commerce 2.3.5不支援AmazonSales Channel4.0.0。若要取得Adobe Commerce 2.3.5的支援，請升級至AmazonSales Channel4.1.0。

![新增](../assets/new.svg) 推出 [AmazonSales Channel](amazon-sales-channel-home.md) 首頁，改善了商店資訊的「卡片檢視」。

![新增](../assets/new.svg) 推出 [儲存儀表板](amazon-store-dashboard.md) 包含清單、最近訂購和儲存設定資訊。

![新增](../assets/new.svg) 導入更簡單、流線型 [上線程式](amazon-onboarding-home.md) 和 [預設存放區設定](default-store-settings.md) 讓您的商店更快整合。

![已知問題](../assets/bug.svg) <!--CHAN-4102--> 當 [建立屬性](managing-attributes.md) 從清單匯入影像和 **儲存檢視** 設為 `All Store Views (Global)`，會造成影像無法匯入至所有商店檢視的已知問題。 如果您變更 **儲存檢視（將值匯入）** 匯入至特定商店的影像。

## v3.0.1

*2019年11月11日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修正](../assets/fix.svg) **數值欄位設定**: <!--CHAN-3779-->需要數值的欄位已更新，僅接受數值字元。 範例：定價規則設定>調整金額欄位

![修正](../assets/fix.svg) **使用手冊連結**: <!--CHAN-3778-->錯誤 _使用手冊_ 連結已修正。

![修正](../assets/fix.svg) **複製Amazon清單**: <!--CHAN-3593-->系統現在已修正先前回報而造成重複Amazon清單的問題。 在此版本之前，擴充功能已將Amazon地區的國家/地區代碼新增至匯入清單時的SKU值。 清單與目錄項目相符，但擴充功能建立了新的重複清單，並附加了SKU。 在此版本中，擴充功能不會修改匯入清單的SKU，且不會變更現有清單。 您可以使用 [!UICONTROL End Listing(s)] 在Amazon選項中移除重複清單。

## v3.0.0

*2019年10月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新增](../assets/new.svg) **Amazon UK Marketplace現已推出**:建立和整合商務商店時，使用者可選擇英國市場。 此英國升級包括對以下項目的額外支援：

- [Amazon增值稅計算服務](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [產品稅碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} 資訊。

![新增](../assets/new.svg) **改善記錄功能**: <!--CHAN-3642, 3672-->實作 **啟用偵錯記錄** 功能，以在需要進行疑難排解時收集其他同步資料。 請參閱 [Sales Channel設定](https://docs.magento.com/user-guide/configuration/sales-channels/global-settings.html) 配置參考中的主題。

![修正](../assets/fix.svg) **產品目錄**: <!--CHAN-3687-->修正因Amazon清單匯入的影像無法套用至對應商務目錄產品的問題。

![修正](../assets/fix.svg) **訂單建立**: <!--CHAN-3708-->修正商務無法為不符合商務目錄產品的Amazon訂單建立訂單的問題。

![已知問題](../assets/bug.svg) **複製Amazon清單**: <!--CHAN-3593-->此問題會導致目錄使用相同的SKU，為匯入的清單建立項目，但結尾會新增地區代碼。 接著，Amazon會將修改後的SKU處理為新項目，並建立清單。 此問題將在未來版本中解決。

## v2.0.0

[!BADGE 相容性]{type=Informative tooltip="相容性"}

>[!NOTE]
>
>1.0.0版僅限有限版本提供。

![新增](../assets/new.svg)  **簡化入門和維護**:透過逐步程式新增及整合您的Amazon賣家帳戶，並透過管理員取得詳細指示。 透過一個控制面板維護您的商店、帳戶和列出的產品。

![新增](../assets/new.svg)  **多帳戶支援**:透過管理員管理並監控多個Amazon品牌和市集地區。

![新增](../assets/new.svg)  **智慧定價**:設定自動重新定價規則，以增加您獲得令人垂涎的Buy Box的機會。 設定價格以根據當前Buy Box價格或最低競爭者定價進行動態調整。 設定限制以重新定價以保護利潤。

![新增](../assets/new.svg)  **清單管理**:使用上市規則自動化產品清單，並將您的商務目錄同步至Amazon Marketplace。 添加特定覆蓋以精確控制您的產品。 直接從管理員監控及管理所有清單。

![新增](../assets/new.svg)  **一致的Inventory management**:持續同步您的商務和Amazon庫存數量。

![新增](../assets/new.svg)  **訂單和履行管理**:透過控制面板追蹤Amazon訂單，提供順暢的通訊和庫存更新。 完成並跟蹤由Amazon、已履行的商家或多種方法履行的訂單發運。

![已知問題](../assets/bug.svg)  更新產品數量時，您可能會遇到等待時間更長的問題。 產品數量的更新可能需要約兩小時才會同步。

![已知問題](../assets/bug.svg)  導入的訂單可能具有 _Prime_ 或 _Premium_ 訂購。 您應在Amazon賣家帳戶中驗證這些訂單。

![已知問題](../assets/bug.svg)  不符合資格的套件產品可能會顯示為符合在Amazon上列出的資格。 捆綁產品中的其中一項產品可能不符合條件。 如果您遇到問題，請檢查捆綁產品項目的資格狀態。

![已知問題](../assets/bug.svg)  使用Inventory management for Commerce 2.3.x時，建立訂單時可能不會觸發部分股票重新索引。 可出售數量會每小時重新計算，這可能會在此更新間隔內導致超銷。
