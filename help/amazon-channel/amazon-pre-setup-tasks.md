---
title: 預先設定任務
description: 在整合Adobe Commerce或Amazon中的Magento Open Source存放區之前，請先檢閱要完成的必要工作。
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 2c753ec5f6f4cd509e61b4875e09e9a1a2577ee7
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# 預先設定任務

之前 [商店整合](./store-integration.md)，您必須確保 [!DNL Amazon Seller Central] 帳戶和 [!DNL Commerce] 帳戶已準備好進行整合。 若要成功整合，有一些必要的預先設定工作。

當您在Amazon銷售管道中設定第一個Amazon商店時，會顯示設定工作的清單。 建議您先檢閱這些工作，再執行 [新增Amazon商店](./store-integration.md). 新增第一家商店後，您可以在Amazon銷售管道的「學習與準備」檢視中檢閱這些工作 [首頁](./amazon-sales-channel-home.md).

## 1.啟用 [!DNL Commerce]

之間同步的所有產品和資料 [!DNL Commerce] 而Amazon是由 [cron job](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}。 當您完成新增或更新清單以及接收訂單等工作時，cron工作會在您的 [!DNL Commerce] 後端和 [!DNL Amazon Seller Central] 帳戶。

- [啟用 [!DNL Commerce] cron](https://docs.magento.com/user-guide/system/cron.html){target=&quot;_blank&quot;}。

- 為獲得最佳效能， [set [!DNL Commerce] cron](https://docs.magento.com/user-guide/configuration/advanced/system.html){target=&quot;_blank&quot;}，每五分鐘執行一次。

## 2.建立 [!DNL Amazon Seller Central] 帳戶

在開始設定Amazon銷售管道之前，您必須具備有效 [!DNL Amazon Seller Central] 帳戶。 若您的 [北美（美國、加州、MX）](https://sell.amazon.com/){target=&quot;_blank&quot;}或 [歐洲（英國）](https://sell.amazon.co.uk/sell-online/beginners-guide){target=&quot;_blank&quot;}區域，您可以完成Amazon的賣方帳戶設定程式。

Amazon銷售管道需要 [!DNL Professional Seller] 帳戶 [!DNL Amazon Seller Central]. Amazon每月收取訂購費和銷售費。 請參閱 [Amazon:選擇您的銷售計畫](https://sell.amazon.com/pricing.html){target=&quot;_blank&quot;}。

## 3.確認您為Amazon認可賣家

若要整合，您必須取得核准 [!DNL Amazon Seller Central] 帳戶。 您的帳戶對產品或類別不得有任何限制。 建立清單之前，有些產品和類別需要獲得批准。 檢閱Amazon的類別和產品核准政策，確保產品獲得核准。 請參閱 [Amazon:需要批准的類別和產品](https://sellercentral.amazon.com/gp/help/200333160){target=&quot;_blank&quot;}（需要賣方中央登錄）。

也請務必確認您已在 [!DNL Amazon Seller Central] 帳戶：

- 確保您的回訪政策與Amazon回訪政策一樣好或更好。 請參閱 [Amazon:返回策略](https://www.amazon.com/gp/help/customer/display.html){target=&quot;_blank&quot;}。

- 確保已配置稅務設定。 請參閱 [Amazon:稅收政策](https://sellercentral.amazon.com/gp/help/external/help.html){target=&quot;_blank&quot;}（需要賣方中央登錄）。

- 請確定您的運送方法已正確設定。 要設定發運方法， [!DNL Commerce] 提供給客戶以履行Amazon訂單，請更新 [Amazon:運送設定](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target=&quot;_blank&quot;} [!DNL Amazon Seller Central] 帳戶。

## 4.確認您的VAT已針對您的商店進行設定

（主要供英國銷售商使用。） Amazon建議您註冊 [Amazon增值稅計算服務](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target=&quot;_blank&quot;}。 如果您選擇不同的方法，則需對增值稅合規性負責。

>[!NOTE]
>
>Amazon可能需要10到14天的時間來驗證和啟用您的增值稅計算服務帳戶。

## 5.增加自動目錄比對的數量

在上線期間，Amazon銷售管道會使用產品屬性，將您現有的Amazon清單（若適用）與您 [!DNL Commerce] 目錄。 上線後，這些產品屬性將用來發佈 [!DNL Commerce] 目錄項目至Amazon清單，並在 [!DNL Commerce] 和Amazon。

若要具有 [!DNL Commerce] 產品會自動與Amazon清單相符，您應為 [!DNL Commerce] 目錄。 設定Amazon銷售管道商店之前，您應先新增 [!DNL Commerce] 產品屬性以符合這些Amazon屬性，例如：ASIN、EAN、ISBN、UPC或GCID。 請參閱 [在中建立產品屬性 [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6.設定您的貨幣和轉換（視需要）

如果您的Amazon商店使用的貨幣與針對 [!DNL Commerce] 商店， [啟用貨幣](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target=&quot;_blank&quot;}並設定 [貨幣兌換率](https://docs.magento.com/user-guide/stores/currency-update.html){target=&quot;_blank&quot;}。

## 7.建立產品條件屬性（視需要）

如果您的Amazon清單包含多個產品條件(例如 _new_, _used_，或 _贊_)，建立 [!DNL Commerce] 屬性和指派條件值。 在上線期間，您必須對應此屬性至Amazon條件產品屬性。 請參閱 [建立Amazon的屬性](./ob-creating-magento-attributes.md).

## 8.設定 [!DNL Amazon Seller Central] 裝運方法

要設定要為履行Amazon訂單提供的發運方法，請參閱 [設定與運送設定][10] 在 [!DNL Amazon Seller Central] 帳戶。

## 其他配置

當您的Amazon帳戶設定並啟用時，有幾個 [!DNL Commerce] 有助於簡化Amazon銷售管道入門流程的建議。

### 檢閱並記下您要排除的任何產品

您可能不想在Amazon上列出某些產品。 Amazon銷售管道有一個清單規則引擎，可用來判斷哪些產品符合發佈至Amazon的資格。 [上市規則](./listing-rules.md) 可讓您選取要發佈（或未發佈）至您的產品子集 [!DNL Amazon Seller Central] 帳戶，例如依類別選擇或定義一或多個產品屬性。 贊 [!DNL Commerce] [目錄](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target=&quot;_blank&quot;}或 [購物車](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target=&quot;_blank&quot;}價格規則，用於Amazon清單資格的產品屬性必須具有 **[!UICONTROL Use for Promo Rule Conditions]** 設為 `Yes`. 請參閱 **[!UICONTROL Use for Promo Rule Conditions]** in [產品屬性](https://docs.magento.com/user-guide/stores/attributes-product.html){target=&quot;_blank&quot;}。

### 設定您的 [!DNL Amazon Seller Central] 非活動地區

為協助您在整合期間進行無錯誤的資料轉換，建議您將Amazon地區設為 `Inactive` 狀態位於「設定>帳戶資訊>假期設定」。 請參閱 [Amazon:假期的清單狀態][11]. 完成設定後，將狀態變回 `Active` 在Amazon。

![下一個表徵圖](assets/btn-next.png) [**繼續建立 [!DNL Commerce] 屬性**](./ob-creating-magento-attributes.md)
