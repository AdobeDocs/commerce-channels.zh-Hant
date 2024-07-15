---
title: ' [!DNL Amazon sales channel]的預先設定工作'
description: 在AmazonSales Channel中整合Adobe Commerce或Magento Open Source存放區之前，請先檢閱要完成的必要工作。
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# [!DNL Amazon sales channel]的預先設定工作

在[存放區整合](./store-integration.md)之前，您必須確定您的[!DNL Amazon Seller Central]帳戶和[!DNL Commerce]帳戶已準備好進行整合。 為了成功整合，有一些必要的預先設定工作。

當您在Amazon sales channel中設定第一個Amazon商店時，設定工作清單隨即出現。 建議您在[新增Amazon市集](./store-integration.md)之前檢閱這些工作。 新增第一個商店後，您可以在Amazon銷售管道[首頁](./amazon-sales-channel-home.md)的「學習與準備」檢視中檢閱這些工作。

## 1.在[!DNL Commerce]中啟用背景工作

所有在[!DNL Commerce]和Amazon之間同步的產品和資料都由[cron工作](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)管理。 當您完成新增或更新清單及接收訂單等工作時，cron工作會在您的[!DNL Commerce]後端與[!DNL Amazon Seller Central]帳戶之間傳送及接收資料。

- [啟用 [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html)。

- 為了達到最大效能，[設定 [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html)每五分鐘執行一次。

## 2.建立您的[!DNL Amazon Seller Central]帳戶

開始設定Amazon銷售管道前，您必須擁有有效的[!DNL Amazon Seller Central]帳戶。 如果您在[北美（美國、CA、MX）](https://sell.amazon.com/){target="_blank"}或[歐洲（英國）](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"}區域沒有現有的Amazon賣家帳戶，您可以完成Amazon的賣家帳戶設定程式。

Amazon sales channel需要[!DNL Amazon Seller Central]上的[!DNL Professional Seller]帳戶。 Amazon每月會收取訂閱及銷售費用。 請參閱[Amazon：選擇您的銷售計畫](https://sell.amazon.com/pricing.html){target="_blank"}。

## 3.確認您是獲得核准的Amazon賣家

若要整合，您必須擁有已核准的[!DNL Amazon Seller Central]帳戶。 您的帳戶對產品或類別不得有任何限制。 有些產品和類別在建立清單之前需要核准。 檢閱類別和產品核准的Amazon政策，確保您的產品獲得核准。 檢視[Amazon：需要核准的類別和產品](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} （需要賣家中心登入）。

同樣重要的是，請確定您已在[!DNL Amazon Seller Central]帳戶中設定下列專案：

- 確認您的退貨政策與Amazon退貨政策相同或更好。 請參閱[Amazon：傳回原則](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}。

- 確定已設定您的稅捐設定。 請參閱[Amazon：稅務政策](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} （需要賣家中心登入）。

- 請確定您的送貨方式已正確設定。 若要設定[!DNL Commerce]提供給客戶的送貨方式，以履行您的Amazon訂單，請更新[!DNL Amazon Seller Central]帳戶中的[Amazon：送貨設定](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"}。

## 4.確定已為商店設定您的VAT

（主要由英國賣家使用。） Amazon建議註冊[Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}。 若您選擇不同的方式，則您需負責VAT規定。

>[!NOTE]
>
>Amazon可能需要10到14天的時間來驗證及啟用您的VAT計算服務帳戶。

## 5.增加自動目錄相符專案的數量

上線期間，Amazon銷售管道會使用產品屬性，將您現有的Amazon清單（如果適用）比對至您[!DNL Commerce]目錄中的現有產品。 上線後，這些產品屬性會用來將您的[!DNL Commerce]目錄專案發佈到Amazon清單，以及在[!DNL Commerce]和Amazon之間同步您的產品資料。

若要讓[!DNL Commerce]個產品的最大數量自動符合Amazon清單，您應該為您的[!DNL Commerce]目錄建立一組產品屬性。 設定Amazon銷售管道存放區之前，您應該新增[!DNL Commerce]產品屬性以符合這些Amazon屬性，例如：ASIN、EAN、ISBN、UPC或GCID。 請參閱[在 [!DNL Commerce]](./ob-creating-magento-attributes.md)中建立產品屬性。

## 6.視需要設定貨幣和轉換

如果您的Amazon商店使用的貨幣與[!DNL Commerce]商店設定的貨幣不同，請[啟用貨幣](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html)並設定[貨幣轉換率](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html)。

## 7.建立產品條件屬性（視需要）

如果您的Amazon清單包含多個產品條件（例如&#x200B;_new_、_used_&#x200B;或&#x200B;_like new_），請建立[!DNL Commerce]屬性並指派條件值。 上線期間，您必須將此屬性對應至Amazon條件產品屬性。 請參閱[建立Amazon的屬性](./ob-creating-magento-attributes.md)。

## 8.設定您的[!DNL Amazon Seller Central]送貨方法

若要設定您想要提供的送貨方式，以符合您的Amazon訂單，請參閱[!DNL Amazon Seller Central]帳戶中的&#x200B;_設定與送貨設定_。

## 其他設定

設定並啟用您的Amazon帳戶時，有數個[!DNL Commerce]建議可協助簡化Amazon銷售管道上線流程。

### 檢閱並記下您要排除的任何產品

您可能不希望某些產品列在Amazon上。 Amazon sales channel有一個清單規則引擎，用來判斷哪些產品符合發佈至Amazon的資格。 [清單規則](./listing-rules.md)可讓您選取要發佈（或未發佈）至您[!DNL Amazon Seller Central]帳戶的產品子集，例如依類別選取或定義一或多個產品屬性。 如同[!DNL Commerce] [目錄](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html)或[購物車](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html)價格規則，用於Amazon清單資格的產品屬性必須將&#x200B;**[!UICONTROL Use for Promo Rule Conditions]**&#x200B;設定為`Yes`。 檢視[產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)中的&#x200B;**[!UICONTROL Use for Promo Rule Conditions]**。

### 將您的[!DNL Amazon Seller Central]區域設定為非使用中

為協助在整合期間進行無錯誤資料轉換，建議您在「設定>帳戶資訊>假期設定」中，將Amazon區域設為`Inactive`狀態。 完成設定後，請在Amazon中將狀態變更回`Active`。

![下一個圖示](assets/btn-next.png) [**繼續建立[!DNL Commerce]屬性**](./ob-creating-magento-attributes.md)
