---
title: '[!DNL Amazon Sales Channel]發行說明'
description: 檢閱發行說明，瞭解所有 [!DNL Amazon Sales Channel] 發行版本的相關資訊。
feature: Sales Channels, Release Notes
exl-id: 792782e0-9097-42f7-9fc0-509ece02e407
source-git-commit: df8bbec23d34b53a0e694c924aca5b1ed41e4d08
workflow-type: tm+mt
source-wordcount: '2010'
ht-degree: 0%

---

# [!DNL Amazon Sales Channel]發行說明

>[!IMPORTANT]
>
> [!DNL Amazon sales channel]可安裝在雲端基礎結構版本2.3.x和2.4.x上具有Magento Open Source、Adobe Commerce和Adobe Commerce的執行個體上。Adobe Commerce 2.1、Magento Open Source2.2或Magento1不再支援此擴充功能。
> <br>僅在Adobe Commerce 2.3.x版本上支援[!DNL Amazon sales channel]版本4.0.0和4.1.0。
> <br>[!DNL Amazon sales channel] 版本4.2.0+與Adobe Commerce 2.3.x版本相容，但僅支援Adobe Commerce 2.4.x版本。
>

這些版本說明說明[!DNL Amazon sales channel]的初始版本，包括：

![新](../assets/new.svg)新功能
![已修正問題](../assets/fix.svg)修正和改良
![已知問題](../assets/bug.svg)已知問題

如需版本設定、支援和相容性，請參閱[即將發行的版本](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html)。

請參閱[產品可用性](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html)，瞭解哪些Adobe Commerce版本支援此擴充功能。

## v4.5.0

*2023年8月30日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新](../assets/new.svg)已新增Adobe.IO API閘道（從MAGI變更），以改善驗證安全性。 `ServicesId`提供新的UI來管理您的Adobe.IO認證，類似於其他[Adobe Commerce服務](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html)。

>[!NOTE]
>
>商戶必須確定已針對生產更新[私人與公開API金鑰](https://experienceleague.adobe.com/docs/commerce-admin/config/services/saas.html)。


![已修正問題](../assets/fix.svg)已識別組態設定問題並修正訂單建立流程。

## v4.4.4

*2023年3月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![已修正問題](../assets/fix.svg)已新增Adobe Commerce 2.4.6和PHP 8.2的支援。

![已修正問題](../assets/fix.svg)減少記錄檔中的雜訊。

![已修正問題](../assets/fix.svg)改善提取更新的穩定性。

![已修正問題](../assets/fix.svg)已簡化執行單一動作（如提取）或從CLI套用的程式。

![已修正問題](../assets/fix.svg)已升級`magento/services-connector`的相依性。

![已修正問題](../assets/fix.svg)已修正具有無效國碼之英國帳戶的同步問題。

![已修正問題](../assets/fix.svg)目錄產品實體的entity_type_id以硬式編碼撰寫會導致Magento價格Source發生問題。

![已修正問題](../assets/fix.svg)已修正從其他執行個體後端刪除的帳戶無法從UI刪除的問題。

![已修正問題](../assets/fix.svg)已修正某些購物車規則中斷訂單匯入的問題。

## v4.4.3

*2023年3月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg)已新增對Adobe Commerce 2.4.4的支援。

## v4.4.2

*2021年11月11日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg)已更新相依性以支援其他更新的擴充功能。
![Fix](../assets/fix.svg)已新增對PHP 8.1的支援。

## v4.4.1

*2021年11月11日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg)已變更Adobe Commerce從Amazon接收&#x200B;_使用者名稱_&#x200B;欄位的方式。 先前，_使用者名稱_&#x200B;欄位包含特殊字元時，建立訂單時發生錯誤。 Adobe Commerce現在會收到&#x200B;_使用者名稱_&#x200B;資料，並篩選掉特殊字元，以便成功建立訂單。

## v4.4.0

*2021年4月9日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新](../assets/new.svg)已新增對設定唯讀模式的支援。 請參閱[銷售管道設定](sales-channel-settings.md)。

![修正](../assets/fix.svg)已變更資料流程，以便相同執行個體的多個復本可同時擷取更新。

![修正](../assets/fix.svg)已變更同步處理帳戶資訊的同步處理序。 新增cron作業以與遠端帳戶同步，並在CLI命令中新增相同的功能。

![Fix](../assets/fix.svg)已新增CLI命令引數和旗標，以取得更精確的控制。

![修正](../assets/fix.svg)修正了系統組態中的背景工作(cron) Source。

![修正](../assets/fix.svg)修正當國碼設定為波多黎各(PR)時，無法建立訂單的問題。

## v4.3.0

*2021年3月3日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) <!--CHAN-xxxx-->已重新設計&#x200B;_訂單詳細資料_&#x200B;功能，不再依賴&#x200B;_匯入訂單_&#x200B;設定。 現在，所有訂單的訂單詳細資料都會顯示在AmazonSales Channel介面中。

![修正](../assets/fix.svg)在Admin的&#x200B;_[!UICONTROL Marketing]_功能表中，名稱已從_[!UICONTROL Amazon]_&#x200B;變更為&#x200B;_[!UICONTROL Amazon Sales Channel]_。

![已知問題](../assets/bug.svg) **重要**： Adobe Commerce 2.4.0相容性的已知問題已在Adobe Commerce 2.4.1版本中解決。

- Amazon cron處理序處於`error`狀態
- 在資料庫中建立存放區時，使用Commerce 2.4.0安裝會失敗
- 安裝MSI時，建立產品失敗

## v4.2.0

*2021年3月3日*

[!BADGE 支援]{type=Informative tooltip="支援"}

如果您已安裝先前的[!DNL Amazon sales channel]版本，並嘗試將Adobe Commerce更新至2.4.0版，在您完成Adobe Commerce更新之前，系統會提示您更新擴充功能。

![已知問題](../assets/bug.svg)當[!DNL Amazon sales channel] 4.2.0與2.4.0版整合且啟用[Inventory management](https://experienceleague.adobe.com/docs/commerce-admin/inventory/introduction.html?lang=en)時，有一個已知問題阻止在您的Commerce目錄中新增產品。 此問題將在未來的Commerce版本中解決。

![新的](../assets/new.svg) [!DNL Amazon sales channel]已增強，可以接受文字型位址資料，並將其與標準化的位址格式比對，包括城市、州/省和郵遞區號。 此更新可讓訂單和運送資料與Amazon同步（同步），而不會出現地址錯誤。<br/>例如，購物者輸入城市、州/省、郵遞區號為`Escondido, californiA 92025-1501`。 AmazonSales Channel會匯入資料並將資料以`Escondido, CA 92025`格式與標準格式比對，然後以此標準化格式將其同步回Amazon。

![新](../assets/new.svg)已新增對PHP 7.4的支援。

![新](../assets/new.svg) <!--CHAN-4334-->已新增Adobe Commerce 2.4.x的支援。舊版可能與Commerce 2.4.x相容，但不受支援。 如需版本相容性，請參閱[即將發行的版本](https://experienceleague.adobe.com/docs/commerce-operations/release/planning/schedule.html)。 必須先將AmazonSales Channel更新至4.2.0，才能完成Adobe Commerce 2.4.0更新。

![修正](../assets/fix.svg) <!--CHAN-4431-->已修正造成UK客戶發生&#x200B;_拒絕存取_&#x200B;錯誤的問題。

![修正](../assets/fix.svg) <!--CHAN-4394-->修正導致Amazon送貨狀態無法同步至對應Commerce訂單的問題，因此Commerce將訂單的送貨狀態「鎖定」為`Pending`，Amazon則是`Unshipped`。 透過新的標準化地址功能，這些送貨狀態錯誤已解決。

![修正](../assets/fix.svg) <!--ticket#-->已更新訂單同步處理（同步），以忽略失敗的訂單匯入，因此可減少多次同步處理嘗試，並允許後續的匯入處理，每五分鐘提交一次訂單同步處理要求。 同步錯誤仍記錄在錯誤記錄中，但標籤為「已處理」以允許進一步的記錄功能。 此外，[!DNL Amazon sales channel]現在會自動移除針對無法在Commerce中建立的訂單所收集的多餘資料。

![修正](../assets/fix.svg)已更新錯誤記錄，以收集未攔截例外狀況與擴充功能更新錯誤的詳細資訊。

![修正](../assets/fix.svg) <!--ticket#-->修正因遺失&#x200B;_價格_&#x200B;值而導致&#x200B;_最低價格_&#x200B;資料的初始同步失敗的問題。

![修正](../assets/fix.svg) <!--CHAN-4410-->修正日期範圍欄位留空時，_Amazon訂單_&#x200B;檢視中造成篩選錯誤的問題。

![修正](../assets/fix.svg) <!--CHAN-4439-->已修正導致數量相關庫存與履行同步錯誤的問題。 現在，擴充功能會先向下舍入以小數輸入的數量值，再與Amazon同步。<br/>例如，當商家手動輸入數量`2.5`時，擴充功能會將值四捨五入為`2`，然後將更新的數量與Amazon同步。

## v4.1.0

*2020年5月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![新增](../assets/new.svg) <!--4247, 4230-->已變更訂單匯入程式，以符合Commerce訂單需求。 這些變更修正了Commerce無法為匯入訂單建立對應訂單的問題。 請參閱[管理訂單](managing-orders.md)，以取得訂單封鎖程式和解決方案的資訊。

![新](../assets/new.svg) <!--CHAN-CHAN-4167, 4297, 4311, 4312, 4324-->已更新商店儀表板的&#x200B;_最近訂單_&#x200B;區段，並新增顯示所有Amazon訂單的新&#x200B;_所有訂單_&#x200B;檢視，包括篩選選項和檢視更多訂單的分頁。 檢視[Amazon商店儀表板](amazon-store-dashboard.md)和[檢視Amazon訂單](amazon-orders-all.md)。

![New](../assets/new.svg)已在&#x200B;_[!UICONTROL Recent Orders]_和_[!UICONTROL All Orders]_&#x200B;檢視中新增重新設計的&#x200B;_[!UICONTROL Amazon Orders]_資料表的_[!UICONTROL Order Notes]_&#x200B;資料行。 _[!UICONTROL Order Notes]_告知商家訂單匯入發生問題。 請參閱[檢視Amazon訂單](amazon-orders-all.md)。

![新](../assets/new.svg) <!--CHAN-4013-->已更新產品條件引數，以符合[Amazon已續約](https://sell.amazon.com/programs/renewed)方案。 請參閱[已更新產品](renewed-products.md)。

![新](../assets/new.svg) <!--CHAN-3680-->已更新[Amazon訂單詳細資料](amazon-order-details.md)，以包含Amazon所履行訂單的「一般資料」。 請參閱[履行者](fulfilled-by.md)。

![修正](../assets/fix.svg) <!--CHAN-4069-->修正導致商店卡上圖示扭曲的問題。

![修正](../assets/fix.svg) <!--CHAN-4165-->已更正錯誤，在工作階段逾時後無法顯示&#x200B;_登入_&#x200B;畫面。

![修正](../assets/fix.svg) <!--CHAN-4211-->修正無法將Amazon訂單稅額匯入新Commerce訂單的問題。

![修正](../assets/fix.svg) <!--CHAN-4234-->已修正導致商店控制面板上顯示的收入總計包含`Canceled`或`Error`狀態的訂單的問題。

![修正](../assets/fix.svg) <!--CHAN-4326-->已修正導致訂單匯入錯誤的問題，此錯誤與使用&#x200B;_Magento Shipping_&#x200B;方法建立訂單的協力廠商擴充功能有關。

![修正](../assets/fix.svg) <!--CHAN-4357-->已修正執行cron同步處理時發生錯誤的問題。 CLI命令已新增鎖定，可防止兩個cron作業同時同步。

![修正](../assets/fix.svg)已更新內容安全性原則，以支援Commerce 2.3.5版。

## v4.0.0

*2020年3月25日*

[!BADGE 支援]{type=Informative tooltip="支援"}

>[!IMPORTANT]
>
>Amazon 2.3.5不支援Adobe CommerceSales Channel4.0.0。如需Adobe Commerce 2.3.5的支援，請升級至AmazonSales Channel4.1.0。

![新](../assets/new.svg)推出新的[AmazonSales Channel](amazon-sales-channel-home.md)首頁，其中包含已改善的商店資訊「卡片檢視」。

![新](../assets/new.svg)推出新的[商店儀表板](amazon-store-dashboard.md)，其中包含清單、近期訂單及商店設定資訊。

![全新](../assets/new.svg)推出更簡單、簡化的[上線程式](amazon-onboarding-home.md)和[預設商店設定](default-store-settings.md)，讓您的商店更快整合。

![已知問題](../assets/bug.svg) <!--CHAN-4102-->當[建立屬性](managing-attributes.md)以便從清單匯入影像且&#x200B;**存放區檢視**&#x200B;設定為`All Store Views (Global)`時，有一個已知問題阻止將影像匯入到所有存放區檢視。 如果您將&#x200B;**存放區檢視（將值匯入）**&#x200B;的設定變更為特定存放區，則會為該存放區匯入影像。

## v3.0.1

*2019年11月11日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![修正](../assets/fix.svg) **數值欄位設定**： <!--CHAN-3779-->需要數值的欄位已更新為僅接受數值字元。 範例：訂價規則設定>調整金額欄位

![修正](../assets/fix.svg) **使用手冊連結**： <!--CHAN-3778-->已更正不正確的&#x200B;_使用手冊_&#x200B;連結。

![修正](../assets/fix.svg) **重複的Amazon清單**： <!--CHAN-3593-->已更正造成重複Amazon清單的先前回報問題。 在此版本之前，擴充功能在匯入清單時，已將Amazon地區的國家/地區代碼新增至SKU值。 此清單與型錄專案相符，但擴充功能建立了包含附加SKU的新重複清單。 在此版本中，擴充功能不會修改匯入清單的SKU，且不會變更現有清單。 您可以使用Amazon上的[!UICONTROL End Listing(s)]選項來移除重複的清單。

## v3.0.0

*2019年10月7日*

[!BADGE 支援]{type=Informative tooltip="支援"}

![全新](../assets/new.svg) **Amazon UK Marketplace現已推出**：使用者在建立和整合Commerce商店時，可以選擇英國Marketplace。 此英國升級包含下列專案的額外支援：

- [Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources){target="_blank"}

- [產品稅捐代碼](https://sellercentral.amazon.com/gp/help/help.html?itemID=G200794510&amp;language=en_US){target="_blank"}資訊。

![新](../assets/new.svg) **已改善記錄**： <!--CHAN-3642, 3672-->已實作&#x200B;**啟用偵錯記錄**&#x200B;功能，以便在需要疑難排解時收集額外的同步處理資料。 請參閱組態參考中的[Sales Channel設定](https://experienceleague.adobe.com/docs/commerce-admin/config/sales-channels.html)主題。

![修正](../assets/fix.svg) **產品目錄**： <!--CHAN-3687-->已修正無法將含有Amazon清單之匯入的影像套用至對應Commerce目錄產品的問題。

![修正](../assets/fix.svg) **訂單建立**： <!--CHAN-3708-->已修正Commerce無法為不符合Commerce目錄產品的Amazon訂單建立訂單的問題。

![已知問題](../assets/bug.svg) **重複的Amazon清單**： <!--CHAN-3593-->此問題會導致目錄使用相同的SKU為匯入清單建立專案，但會在結尾新增地區代碼。 Amazon接著會將修改過的SKU處理為新專案，並建立清單。 此問題將在未來版本中解決。

## v2.0.0

[!BADGE 支援]{type=Informative tooltip="支援"}

>[!NOTE]
>
>1.0.0版僅在限量版中提供。

![新](../assets/new.svg) **簡化的入門與維護**：透過管理員提供的詳細指示，透過逐步程式新增並整合您的Amazon賣家帳戶。 透過單一儀表板維護您的商店、帳戶和列出的產品。

![新增](../assets/new.svg) **多個帳戶支援**：透過管理員管理及監視多個Amazon品牌和市集區域。

![新的](../assets/new.svg) **智慧型定價**：設定自動重新訂價規則，以增加您夢寐以求的Buy Box機會。 設定價格，以動態調整至目前的Buy Box價格，或最低競爭者價格。 設定重新訂價的上限以保護您的利潤。

![新增](../assets/new.svg) **清單管理**：使用清單規則自動化產品清單，並將您的Commerce目錄同步至Amazon Marketplace。 新增特定覆寫，以精細控制您的方案。 直接從「管理員」監視及管理所有清單。

![新的](../assets/new.svg) **一致的Inventory management**：保持您的Commerce和Amazon庫存數量持續同步。

![新](../assets/new.svg) **訂單與履行管理**：透過儀表板追蹤Amazon訂單，並透過順暢的通訊和存貨更新。 完成並追蹤由Amazon、已履行的商家或多種方法所履行的訂單出貨。

![已知問題](../assets/bug.svg)您可能會遇到更新產品數量的等候時間較長的問題。 產品數量的更新可能需要約兩個小時才能同步。

![已知問題](../assets/bug.svg)匯入的訂單可能有&#x200B;_Prime_&#x200B;或&#x200B;_Premium_&#x200B;訂單的型別。 您應在Amazon賣家帳戶中驗證這些訂單。

![已知問題](../assets/bug.svg)不符合資格的套件產品可能會顯示為「符合在Amazon上列出的資格」。 套件產品中的其中一種產品可能不符合條件。 如果您遇到問題，請檢查套裝產品專案的適用狀態。

![已知問題](../assets/bug.svg)使用適用於Commerce 2.3.x的Inventory management時，建立訂單時可能不會觸發部分股票重新索引。 可銷售數量會每小時重新計算，這可能會導致在此更新間隔期間過度銷售。
