---
title: 預先設定任務
description: 在整合您的Adobe商務或AmazonSales Channel中的Magento Open Source商店之前，請先檢閱要完成的必要工作。
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# 預先設定任務

在[儲存整合](./store-integration.md)之前，您必須確定您的[!DNL Amazon Seller Central]帳戶和[!DNL Commerce]帳戶已準備好進行整合。 若要成功整合，有一些必要的預先設定工作。

當您在Amazon銷售管道中設定第一個Amazon商店時，會顯示設定工作的清單。 建議您在[新增Amazon商店](./store-integration.md)之前檢閱這些工作。 新增第一家商店後，您可以在Amazon銷售管道[首頁](./amazon-sales-channel-home.md)的「學習與準備」檢視中檢閱這些工作。

## 1.在[!DNL Commerce]中啟用後台任務

[!DNL Commerce]與Amazon之間同步的所有產品和資料均由[cron job](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}管理。 當您完成新增或更新清單以及接收訂單等工作時，cron工作會在您的[!DNL Commerce]後端和[!DNL Amazon Seller Central]帳戶之間傳送和接收資料。

- [ [!DNL Commerce] Enablecron](https://docs.magento.com/user-guide/system/cron.html) {target=&quot;_blank&quot;}。

- 要獲得最大效能，請每五分鐘運行一次[set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;}。

## 2.建立您的[!DNL Amazon Seller Central]帳戶

開始設定Amazon銷售管道之前，您必須有有效的[!DNL Amazon Seller Central]帳戶。 如果您在[北美(US, CA, MX)](https://sell.amazon.com/){target=&quot;_blank&quot;}或[歐洲(UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target=&quot;_blank&quot;}區域中沒有現有的Amazon賣方帳戶，您可以完成Amazon賣方帳戶設定程式。

Amazon銷售管道需要[!DNL Amazon Seller Central]上的[!DNL Professional Seller]帳戶。 Amazon每月收取訂購費和銷售費。 請參閱[Amazon:選擇您的銷售計畫](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}。

## 3.確認您為Amazon認可賣家

若要整合，您必須擁有已核准的[!DNL Amazon Seller Central]帳戶。 您的帳戶對產品或類別不得有任何限制。 建立清單之前，有些產品和類別需要獲得批准。 檢閱Amazon的類別和產品核准政策，確保產品獲得核准。 請參閱[Amazon:需要批准的類別和產品](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;}（需要賣方中央登錄）。

也請務必確保您已在[!DNL Amazon Seller Central]帳戶中設定下列項目：

- 確保您的回訪政策與Amazon回訪政策一樣好或更好。 請參閱[Amazon:返回策略](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}。

- 確保已配置稅務設定。 請參閱[Amazon:稅政策](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;}（需要賣方中央登錄）。

- 請確定您的運送方法已正確設定。 要設定向客戶提供[!DNL Commerce]以履行Amazon訂單的發運方法，請更新[Amazon:[!DNL Amazon Seller Central]帳戶中的運送設定](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;}。

## 4.確認您的VAT已針對您的商店進行設定

（主要供英國銷售商使用。） Amazon建議註冊[Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;}。 如果您選擇不同的方法，則需對增值稅合規性負責。

>[!NOTE]
>
>Amazon可能需要10到14天的時間來驗證和啟用您的增值稅計算服務帳戶。

## 5.增加自動目錄比對的數量

在上線期間，Amazon銷售管道會使用產品屬性，將您現有的Amazon清單（若適用）與[!DNL Commerce]目錄中的現有產品相符。 上線後，這些產品屬性可用來將[!DNL Commerce]目錄項目發佈至Amazon清單，以及在[!DNL Commerce]和Amazon之間同步產品資料。

若要讓最多的[!DNL Commerce]產品自動符合Amazon清單，您應為[!DNL Commerce]目錄建立一組產品屬性。 在設定Amazon銷售管道商店之前，您應先新增[!DNL Commerce]產品屬性，以符合這些Amazon屬性，例如：ASIN、EAN、ISBN、UPC或GCID。 請參閱[在 [!DNL Commerce]](./ob-creating-magento-attributes.md)中建立產品屬性。

## 6.設定您的貨幣和轉換（視需要）

如果您的Amazon商店使用的貨幣與為[!DNL Commerce]商店設定的貨幣不同，請[啟用currency](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;}並設定[貨幣轉換率](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;}。

## 7.建立產品條件屬性（視需要）

如果您的Amazon清單包含多個產品條件（例如&#x200B;_new_、_used_&#x200B;或&#x200B;_like new_），請建立[!DNL Commerce]屬性並指派條件值。 在上線期間，您必須對應此屬性至Amazon條件產品屬性。 請參閱[建立Amazon的屬性](./ob-creating-magento-attributes.md)。

## 8.配置[!DNL Amazon Seller Central]發運方法

要設定要為完成Amazon訂單而提供的發運方法，請參閱[!DNL Amazon Seller Central]帳戶中的[設定和發運設定][10]。

## 其他配置

當您的Amazon帳戶設定並處於作用中狀態時，有幾個[!DNL Commerce]建議可協助簡化Amazon銷售管道上線程式。

### 檢閱並記下您要排除的任何產品

您可能不想在Amazon上列出某些產品。 Amazon銷售管道有一個清單規則引擎，可用來判斷哪些產品符合發佈至Amazon的資格。 [清](./listing-rules.md) 單規則可讓您選取要發佈（或未發佈）至帳戶的產 [!DNL Amazon Seller Central] 品子集，例如透過類別選擇或定義一或多個產品屬性。與[!DNL Commerce] [catalog](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;}或[購物車](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}價格規則一樣，用於Amazon清單資格的產品屬性必須將&#x200B;**[!UICONTROL Use for Promo Rule Conditions]**&#x200B;設為`Yes`。 請參閱[產品屬性](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}中的&#x200B;**[!UICONTROL Use for Promo Rule Conditions]**。

### 將您的[!DNL Amazon Seller Central]地區設為非作用中

為協助在整合期間進行無錯誤的資料轉換，建議您在「設定>帳戶資訊>度假設定」中將Amazon地區設為`Inactive`狀態。 請參閱[Amazon:列出假期的狀態][11]。 完成設定後，將Amazon中的狀態變回`Active`。

![下一](assets/btn-next.png) [**個圖示繼續建立屬 [!DNL Commerce] 性**](./ob-creating-magento-attributes.md)
