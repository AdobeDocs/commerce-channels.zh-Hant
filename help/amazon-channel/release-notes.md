---
title: '"[!DNL Amazon Sales Channel] 發行說明'''
description: 查看發行說明以瞭解有關所有 [!DNL Amazon Sales Channel] 版本。
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: 3b2f60ad2796ee1fdc8808fc0941d76a603b2213
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 0%

---

# 發行說明

>[!IMPORTANT]
>
> [!DNL Amazon sales channel] 可以安裝在雲基礎架構版本2.3.x和2.4.x上具有Magento Open Source、Adobe Commerce和Adobe Commerce的實例上。Adobe Commerce2.1、Magento Open Source2.2或Magento1不再支援擴展。
> <br>支援 [!DNL Amazon sales channel]  僅Adobe Commerce2.3.x版4.0.0和4.1.0版。
> <br>[!DNL Amazon sales channel] 4.2.0+版與Adobe Commerce2.3.x版相容，但僅支援Adobe Commerce2.4.x版。

本發行說明描述了 [!DNL Amazon sales channel] 包括：

![新建](../assets/new.svg) 新功能
![已修復問題](../assets/fix.svg) 修復和改進
![已知問題](../assets/bug.svg) 已知問題

請參閱 [即將發佈的版本](https://devdocs.magento.com/release/){target="_blank"} 用於版本控制、支援和相容性。

## v4.4.4

*2023年3月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![已修復問題](../assets/fix.svg) 增加對Adobe Commerce2.4.6和八點二菲律賓比索的支援。

![已修復問題](../assets/fix.svg) 減少日誌中的噪音。

![已修復問題](../assets/fix.svg) 提拉更新的穩定性得到提高。

![已修復問題](../assets/fix.svg) 簡化了運行單個類似操作的拉式或從CLI應用的過程。

![已修復問題](../assets/fix.svg) 已升級的 `magento/services-connector`。

![已修復問題](../assets/fix.svg) 已修復國家/地區代碼無效的英國帳戶中的同步問題。

![已修復問題](../assets/fix.svg) 硬編碼目錄產品實體的entity_type_id會導致Magento價格源問題。

![已修復問題](../assets/fix.svg) 已更正防止從另一個實例刪除的後端帳戶從UI中刪除的問題。

![已修復問題](../assets/fix.svg) 解決了某些購物車規則違反訂單導入的問題。

## v4.4.3

*2023年3月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修復](../assets/fix.svg) 增加了對Adobe Commerce2.4.4的支援。

## v4.4.2

*2021年11月11日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修復](../assets/fix.svg) 已更新依賴項以支援其他更新的擴展。
![修復](../assets/fix.svg) 添加了對八點一菲律賓比索的支援。

## v4.4.1

*2021年11月11日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修復](../assets/fix.svg) 更改了Adobe Commerce接收 _用戶名_ 從Amazon。 以前，在建立訂單時 _用戶名_ 欄位包含特殊字元。 Adobe Commerce現在收到 _用戶名_ 並過濾出特殊字元，以便成功建立訂單。

## v4.4.0

*2021年4月9日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新建](../assets/new.svg) 為配置添加了對只讀模式的支援。 請參閱 [銷售渠道設定](sales-channel-settings.md)。

![修復](../assets/fix.svg) 已更改資料流，以便同一實例的多個副本可以同時獲取更新。

![修復](../assets/fix.svg) 已更改同步帳戶資訊的同步進程。 已添加要與遠程帳戶同步的cron作業，並將相同的功能添加到CLI命令。

![修復](../assets/fix.svg) 已添加CLI命令參數和標誌，以實現更精確的控制。

![修復](../assets/fix.svg) 已更正系統配置中的後台任務(cron)源。

![修復](../assets/fix.svg) 更正了在將國家法規設為波多黎各時，妨礙訂單的問題。

## v4.3.0

*2021年3月3日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修復](../assets/fix.svg) <!--CHAN-xxxx-->的 _訂單詳細資訊_ 功能已經重新設計，不再依賴 _導入訂單_ 的子菜單。 訂單詳細資訊現在顯示在所有訂單的AmazonSales Channel介面中。

![修復](../assets/fix.svg) 在 _[!UICONTROL Marketing]_菜單，名稱已從_[!UICONTROL Amazon]_ 至 _[!UICONTROL Amazon Sales Channel]_。

![已知問題](../assets/bug.svg) **重要**:Adobe Commerce相容性2.4.0已知問題在Adobe Commerce版中2.4.1解。

- Amazon克龍過程 `error` 狀態
- 在資料庫中建立儲存時，使用Commerce 2.4.0進行安裝失敗
- 安裝MSI時建立產品失敗

## v4.2.0

*2021年3月3日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

如果你之前 [!DNL Amazon sales channel] 版本已安裝並嘗試將您的Adobe Commerce更新為2.4.0版，系統會提示您更新擴展，然後您才能完成Adobe Commerce更新。

![已知問題](../assets/bug.svg) 當 [!DNL Amazon sales channel] 4.2.0與2.4.0版整合， [Inventory management](https://docs.magento.com/user-guide/catalog/inventory.html) 啟用時，會出現一個已知問題，該問題會阻止在您的Commerce目錄中添加產品。 此問題將在未來的Commerce版本中解決。

![新建](../assets/new.svg) [!DNL Amazon sales channel] 已增強，以接受基於文本的地址資料並將其與標準化地址格式（包括城市、州和郵遞區號）匹配。 此更新使訂單和發運資料能夠與Amazon同步（同步），而無地址錯誤。<br/>例如，購物者將市、州、郵遞區號輸入 `Escondido, californiA 92025-1501`。 AmazonSales Channel導入資料並將資料與標準格式匹配 `Escondido, CA 92025`，然後以標準化格式將其同步回Amazon。

![新建](../assets/new.svg) 增加了對七點四菲律賓比索的支援。

![新建](../assets/new.svg) <!--CHAN-4334-->增加對Adobe Commerce2.4.x的支援。以前的版本可能與Commerce 2.4.x相容，但不受支援。 請參閱 [即將發佈的版本](https://devdocs.magento.com/release/){:target=&quot;_blank&quot;}，以瞭解版本相容性。 AmazonSales Channel必須更新4.2.0，才能完2.4.0Adobe Commerce更新。

![修復](../assets/fix.svg) <!--CHAN-4431-->已更正導致 _拒絕訪問_ 英國客戶出錯。

![修復](../assets/fix.svg) <!--CHAN-4394-->已更正導致Amazon裝運狀態無法同步到相應的商務訂單的問題，從而將訂單的裝運狀態「鎖定」為 `Pending` 在商業和 `Unshipped` 在Amazon。 使用新的標準化地址功能，這些發運狀態錯誤已得到解決。

![修復](../assets/fix.svg) <!--ticket#-->已更新訂單同步（同步）以忽略失敗的訂單導入，因此減少了多次同步嘗試並允許後續導入處理，訂單同步請求每五分鐘提交一次。 同步錯誤仍記錄在錯誤日誌中，但標籤為「已處理」以允許進一步記錄功能。 還有， [!DNL Amazon sales channel] 現在自動刪除為未能在Commerce中建立的訂單收集的多餘資料。

![修復](../assets/fix.svg) 已更新錯誤記錄以收集未捕獲異常和擴展更新錯誤的詳細資訊。

![修復](../assets/fix.svg) <!--ticket#-->已更正導致初始同步的問題 _最低價_ 資料因丟失而失敗 _價格_ 值。

![修復](../assets/fix.svg) <!--CHAN-4410-->已更正導致 _Amazon訂單_ 查看日期範圍欄位保留為空的時間。

![修復](../assets/fix.svg) <!--CHAN-4439-->已更正導致與數量相關的庫存和完成同步錯誤的問題。 現在，在與Amazon同步之前，擴展將向下捨入以小數形式輸入的數量值。<br/> 例如，當商家手動輸入 `2.5`，擴展將值向下捨入到 `2` 然後將更新的數量與Amazon同步。

## v4.1.0

*2020年5月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新建](../assets/new.svg) <!--4247, 4230-->已更改訂單導入流程以與Commerce訂單要求保持一致。 這些更改會更正一些問題，這些問題使Commerce無法為導入的訂單建立相應的訂單。 請參閱 [管理訂單](managing-orders.md) 有關訂單攔截器和解決方案的資訊。

![新建](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->已更新 _最近訂單_ 添加新的 _所有訂單_ 顯示所有Amazon訂單的視圖，包括篩選器選項和用於查看更多訂單的分頁。 請參閱 [Amazon商店儀表板](amazon-store-dashboard.md) 和 [查看Amazon訂單](amazon-orders-all.md)。

![新建](../assets/new.svg) 已添加 _[!UICONTROL Order Notes]_重新設計的專欄_[!UICONTROL Amazon Orders]_ 兩個 _[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_ 的子菜單。 _[!UICONTROL Order Notes]_讓商人知道訂單的進口有問題。 請參閱 [查看Amazon訂單](amazon-orders-all.md)。

![新建](../assets/new.svg) <!--CHAN-4013-->更新的產品條件參數以與 [Amazon續約](https://sell.amazon.com/programs/renewed) 的子菜單。 請參閱 [續訂的產品](renewed-products.md)。

![新建](../assets/new.svg) <!--CHAN-3680-->已更新 [Amazon訂單詳細資訊](amazon-order-details.md) 包括Amazon履行的訂單的&quot;通用資料&quot;。 請參閱 [履行者](fulfilled-by.md)。

![修復](../assets/fix.svg) <!--CHAN-4069-->已更正導致儲存卡上表徵圖失真的問題。

![修復](../assets/fix.svg) <!--CHAN-4165-->更正了阻止 _登錄_ 螢幕。

![修復](../assets/fix.svg) <!--CHAN-4211-->更正了阻止Amazon訂單稅額導入新商務訂單的問題。

![修復](../assets/fix.svg) <!--CHAN-4234-->更正了導致商店控制面板上顯示的收入合計包含訂單的問題 `Canceled` 或 `Error` 狀態。

![修復](../assets/fix.svg) <!--CHAN-4326-->已更正導致與使用的第三方擴展關聯的訂單導入錯誤的問題 _Magento Shipping_ 建立訂單的方法。

![修復](../assets/fix.svg) <!--CHAN-4357-->已更正在運行cron同步時導致錯誤的問題。 已在CLI命令中添加了一個鎖，該鎖阻止兩個cron作業同時同步。

![修復](../assets/fix.svg) 已更新內容安全策略，以支援2.3.5版。

## v4.0.0

*2020年3月25日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

>[!IMPORTANT]
>
>Amazon4.0.0不支援Adobe Commerce2.3.5。要獲得Adobe Commerce2.3.5的支援，請升級到AmazonSales Channel4.1.0。

![新建](../assets/new.svg) 引入了 [AmazonSales Channel](amazon-sales-channel-home.md) 首頁，「卡視圖」用於您的商店資訊。

![新建](../assets/new.svg) 引入了 [儲存儀表板](amazon-store-dashboard.md) 清單、最近訂單和儲存設定資訊。

![新建](../assets/new.svg) 引入更簡單、流線型 [聯機](amazon-onboarding-home.md) 和 [預設儲存設定](default-store-settings.md) 讓您的商店更快地整合。

![已知問題](../assets/bug.svg) <!--CHAN-4102--> 當 [建立屬性](managing-attributes.md) 用於從清單和 **儲存視圖** 設定為 `All Store Views (Global)`，存在阻止將影像導入所有儲存視圖的已知問題。 如果更改 **儲存視圖（將值導入）** 將映像導入到特定儲存。

## v3.0.1

*2019年11月11日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![修復](../assets/fix.svg) **數字欄位設定**: <!--CHAN-3779-->需要基於數字的值的欄位已更新為只接受數字字元。 示例：定價規則設定>調整金額欄位

![修復](../assets/fix.svg) **使用手冊連結**: <!--CHAN-3778-->錯誤 _使用手冊_ 連結已更正。

![修復](../assets/fix.svg) **重複的Amazon清單**: <!--CHAN-3593-->以前報告的導致重複的Amazon清單的問題現在已更正。 在此版本之前，擴展在導入清單時將Amazon地區的國家/地區代碼添加到SKU值。 清單與目錄項匹配，但擴展建立了新的、重複的清單，並附加了SKU。 在此版本中，擴展不會修改導入清單的SKU，也不會對現有清單進行任何更改。 您可以使用 [!UICONTROL End Listing(s)] 在Amazon上刪除重複清單。

## v3.0.0

*2019年10月7日*

[!BADGE 相容性]{type=Informative tooltip="相容性"}

![新建](../assets/new.svg) **Amazon英國市場現已推出**:用戶在建立和整合Commerce商店時可以選擇英國市場。 此英國升級包括對以下方面的額外支援：

- [Amazon增值稅計稅服務](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [產品稅碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"} 的下界。

![新建](../assets/new.svg) **改進的日誌記錄**: <!--CHAN-3642, 3672-->已實施 **啟用調試日誌記錄** 功能，可在需要進行故障排除時收集其他同步資料。 查看 [Sales Channel設定](https://docs.magento.com/user-guide/configuration/sales-channels/global-settings.html) 配置參考中的主題。

![修復](../assets/fix.svg) **產品目錄**: <!--CHAN-3687-->更正了阻止使用Amazon清單導入的影像應用到相應的商業目錄產品的問題。

![修復](../assets/fix.svg) **訂單建立**: <!--CHAN-3708-->更正了阻止Commerce為與Commerce目錄產品不匹配的Amazon訂單建立訂單的問題。

![已知問題](../assets/bug.svg) **重複的Amazon清單**: <!--CHAN-3593-->此問題導致目錄為導入的清單建立項目，使用相同的SKU，但最終添加了區域代碼。 Amazon將修改後的SKU作為新項目處理並建立清單。 此問題將在以後的版本中解決。

## v2.0.0

[!BADGE 相容性]{type=Informative tooltip="相容性"}

>[!NOTE]
>
>1.0.0版僅在有限版本中提供。

![新建](../assets/new.svg)  **簡化的登機和維護**:通過逐步過程添加並整合您的Amazon賣家帳戶，並通過管理員提供詳細說明。 通過一個儀表板維護您的商店、帳戶和列出的產品。

![新建](../assets/new.svg)  **多客戶支援**:通過管理員管理和監控多個Amazon品牌和市場區域。

![新建](../assets/new.svg)  **智慧定價**:設定自動重新定價規則以增加您獲得令人垂涎的Buy Box的機會。 設定價格以根據當前Buy Box價格或最低競爭對手的定價動態調整。 將限制設定為重新定價以保護利潤。

![新建](../assets/new.svg)  **清單管理**:使產品清單自動化，並使用上市規則將您的Commerce目錄同步到Amazon市場。 添加特定替代以精細控制您的產品。 直接從管理員監視和管理所有清單。

![新建](../assets/new.svg)  **一致的Inventory management**:保持Commerce和Amazon庫存數量不變的同步。

![新建](../assets/new.svg)  **訂單和履行管理**:通過控制板跟蹤Amazon訂單，實現無縫通信和庫存更新。 完成並跟蹤由Amazon、商家履行或多種方法組合履行的訂單發運。

![已知問題](../assets/bug.svg)  更新產品數量時可能會遇到較長的等待時間。 產品數量的更新可能需要大約兩個小時才能同步。

![已知問題](../assets/bug.svg)  導入的訂單可能具有 _素數_ 或 _高級_ 命令。 您應在Amazon賣家帳戶中驗證這些訂單。

![已知問題](../assets/bug.svg)  不合格的捆綁產品可顯示為符合在Amazon上市的資格。 捆綁產品中的一種產品可能不合格。 如果遇到問題，請檢查捆綁產品項目的資格狀態。

![已知問題](../assets/bug.svg)  當將Inventory management用於Commerce 2.3.x時，在建立訂單時不會觸發部分股票重新指數。 可出售數量會按小時重新計算，這可能導致在此更新間隔期間出現超量銷售。
