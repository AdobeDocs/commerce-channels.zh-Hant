---
title: 預設定任務
description: 在整合Adobe Commerce或AmazonMagento Open Source商店之前，請查看要完成的所需任務。
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 0%

---

# 預設定任務

之前 [儲存整合](./store-integration.md)，您必須確保 [!DNL Amazon Seller Central] 帳戶和 [!DNL Commerce] 帳戶已準備好進行整合。 要成功整合，需要執行一些預設定任務。

當您在Amazon銷售渠道中設定您的第一家Amazon商店時，將顯示安裝任務清單。 建議您先查看這些任務 [添加Amazon商店](./store-integration.md)。 添加第一家商店後，您可以在Amazon銷售渠道的「學習和準備」視圖中查看這些任務 [首頁](./amazon-sales-channel-home.md)。

## 1。在中啟用後台任務 [!DNL Commerce]

在以下時間之間同步的所有產品和資料 [!DNL Commerce] Amazon由 [克倫](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}。 當您完成添加或更新清單和接收訂單等任務時，cron作業會在您的 [!DNL Commerce] 後端 [!DNL Amazon Seller Central] 帳戶。

- [啟用 [!DNL Commerce] 克隆](https://docs.magento.com/user-guide/system/cron.html){target="_blank"}。

- 為了獲得最高效能， [集 [!DNL Commerce] 克隆](https://docs.magento.com/user-guide/configuration/advanced/system.html){target="_blank"} 每五分鐘跑一次。

## 2.建立 [!DNL Amazon Seller Central] 帳戶

在開始設定Amazon銷售渠道之前，您必須具有 [!DNL Amazon Seller Central] 帳戶。 如果您在中沒有現有的Amazon賣家帳戶 [北美（美國，加利福尼亞，墨西哥）](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} 區域，您可以完成Amazon的賣家帳戶設定流程。

Amazon銷售渠道需要 [!DNL Professional Seller] 帳戶 [!DNL Amazon Seller Central]。 Amazon每月收取訂購費和銷售費。 請參閱 [Amazon:選擇銷售計畫](https://sell.amazon.com/pricing.html){target="_blank"}。

## 3.確保你是Amazon的賣家

要整合，必須獲得批准 [!DNL Amazon Seller Central] 帳戶。 您的帳戶不得對產品或類別有任何限制。 某些產品和類別在建立清單之前需要獲得批准。 查看Amazon的類別和產品批准政策，確保您的產品獲得批准。 請參閱 [Amazon:需要批准的類別和產品](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} （需要賣方中心登錄）。

另外，還必須確保在 [!DNL Amazon Seller Central] 帳戶：

- 確保你的回返政策與Amazon的回返政策一樣好或更好。 請參閱 [Amazon:返回策略](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}。

- 確保已配置稅務設定。 請參閱 [Amazon:稅收政策](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} （需要賣方中心登錄）。

- 確保正確配置了您的發運方法。 設定發運方法 [!DNL Commerce] 提供給客戶以履行您的Amazon訂單，更新 [Amazon:裝運設定](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} 在 [!DNL Amazon Seller Central] 帳戶。

## 4.確保為商店配置增值稅

（主要供英國賣家使用。） Amazon建議註冊 [Amazon增值稅計稅服務](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}。 如果您選擇其他方法，則您將負責增值稅合規性。

>[!NOTE]
>
>Amazon可能需要10至14天時間驗證並激活您的增值稅計算服務帳戶。

## 5.增加自動目錄匹配數

在入門期間，Amazon銷售渠道使用產品屬性將您現有的Amazon清單（如果適用）與您的現有產品匹配 [!DNL Commerce] 目錄。 登錄後，這些產品屬性用於發佈 [!DNL Commerce] 將目錄項目列到Amazon清單，並在 [!DNL Commerce] 和Amazon。

具有 [!DNL Commerce] 產品自動與Amazon清單匹配，您應為 [!DNL Commerce] 目錄。 在設定Amazon銷售渠道商店之前，應添加 [!DNL Commerce] 與這些Amazon屬性匹配的產品屬性，例如：ASIN、EAN、ISBN、UPC或GCID。 請參閱 [在中建立產品屬性 [!DNL Commerce]](./ob-creating-magento-attributes.md)。

## 6。配置幣種和轉換（根據需要）

如果您的Amazon商店使用的貨幣與為您的 [!DNL Commerce] 商店， [啟用幣種](https://docs.magento.com/user-guide/configuration/general/currency-setup.html){target="_blank"} and set the [currency conversion rate](https://docs.magento.com/user-guide/stores/currency-update.html){target="_blank"}。

## 7。建立產品條件屬性（根據需要）

如果您的Amazon清單包含多個產品條件(例如 _新_。 _已使用_&#x200B;或 _新_)，建立 [!DNL Commerce] 屬性和賦值條件值。 在載入到「Amazon條件」產品屬性期間，必須映射此屬性。 請參閱 [為Amazon建立屬性](./ob-creating-magento-attributes.md)。

## 8.配置 [!DNL Amazon Seller Central] 運輸方法

要設定要用於履行Amazon訂單的發運方法，請參閱： [設定和裝運設定][10] 在 [!DNL Amazon Seller Central] 帳戶。

## 其他配置

當你的Amazon帳戶設定為活動時，有幾個 [!DNL Commerce] 有助於簡化Amazon銷售渠道的入門流程的建議。

### 複查並記錄要排除的任何產品

您可能不希望某些產品在Amazon上列出。 Amazon銷售渠道有一個清單規則引擎，用於確定哪些產品有資格發佈到Amazon。 [上市規則](./listing-rules.md) 允許您選擇要發佈（或未發佈）到您的產品的子集 [!DNL Amazon Seller Central] 帳戶，如按類別選擇或定義一個或多個產品屬性。 像 [!DNL Commerce] [目錄](https://docs.magento.com/user-guide/marketing/price-rules-catalog.html){target="_blank"} or [shopping cart](https://docs.magento.com/user-guide/marketing/price-rules-cart.html){target="_blank"} price rules, product attributes used for Amazon listing eligibility must have **[!UICONTROL Use for Promo Rule Conditions]** set to `Yes`. See the **[!UICONTROL Use for Promo Rule Conditions]** in [Product Attributes](https://docs.magento.com/user-guide/stores/attributes-product.html){target="_blank"}。

### 設定 [!DNL Amazon Seller Central] 區域至非活動

為幫助在整合期間實現無錯誤的資料過渡，建議您將Amazon地區設定為 `Inactive` 設定>帳戶資訊>假期設定中的狀態。 請參閱 [Amazon:列出假期狀態][11]。 完成設定後，將狀態更改回 `Active` 在Amazon。

![下一個表徵圖](assets/btn-next.png) [**繼續建立 [!DNL Commerce] 屬性**](./ob-creating-magento-attributes.md)
