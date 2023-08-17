---
title: 的預先設定任務 [!DNL Amazon sales channel]
description: 在AmazonSales Channel中整合Adobe Commerce或Magento Open Source存放區之前，請先檢閱要完成的必要工作。
role: Admin, Developer
feature: Sales Channels, Install, Configuration
exl-id: eb9d9136-925f-4b20-9d65-b166173f434b
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 0%

---

# 的預先設定任務 [!DNL Amazon sales channel]

早於 [存放區整合](./store-integration.md)，您必須確保 [!DNL Amazon Seller Central] 帳戶與您的 [!DNL Commerce] 帳戶已準備好進行整合。 為了成功整合，有一些必要的預先設定工作。

當您在Amazon sales channel中設定第一個Amazon商店時，設定工作清單隨即出現。 建議您先檢閱這些工作 [新增Amazon存放區](./store-integration.md). 新增您的第一個商店後，您可以在Amazon銷售管道的「學習與準備」檢視中檢視這些工作 [首頁](./amazon-sales-channel-home.md).

## 1.啟用背景工作 [!DNL Commerce]

所有產品與資料都同步於 [!DNL Commerce] 而Amazon是由 [cron工作](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html). 當您完成新增或更新清單等作業並接收訂單時，cron工作會在您與您的系統之間 [!DNL Commerce] 後端與您的 [!DNL Amazon Seller Central] 帳戶。

- [啟用 [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/systems/tools/cron.html).

- 為達到最佳效能， [設定 [!DNL Commerce] cron](https://experienceleague.adobe.com/docs/commerce-admin/config/advanced/system.html) 每五分鐘執行一次。

## 2.建立您的 [!DNL Amazon Seller Central] 帳戶

在開始設定Amazon銷售管道之前，您必須擁有使用中 [!DNL Amazon Seller Central] 帳戶。 如果您在中沒有現有的Amazon賣家帳戶 [北美（美國、CA、MX）](https://sell.amazon.com/){target="_blank"} or [European (UK)](https://sell.amazon.co.uk/sell-online/beginners-guide){target="_blank"} 地區，您可以完成Amazon的賣家帳戶設定程式。

Amazon銷售管道需要 [!DNL Professional Seller] 帳戶於 [!DNL Amazon Seller Central]. Amazon每月會收取訂閱及銷售費用。 另請參閱 [Amazon：選擇您的銷售計畫](https://sell.amazon.com/pricing.html){target="_blank"}.

## 3.確認您是獲得核准的Amazon賣家

若要整合，您必須擁有核准許可權 [!DNL Amazon Seller Central] 帳戶。 您的帳戶對產品或類別不得有任何限制。 有些產品和類別在建立清單之前需要核准。 檢閱類別和產品核准的Amazon政策，確保您的產品獲得核准。 另請參閱 [Amazon：需要核准的類別和產品](https://sellercentral.amazon.com/gp/help/200333160){target="_blank"} （需要使用Seller Central登入）。

同樣重要的是，請確定您已在 [!DNL Amazon Seller Central] 帳戶：

- 確認您的退貨政策與Amazon退貨政策相同或更好。 另請參閱 [Amazon：回訪政策](https://www.amazon.com/gp/help/customer/display.html){target="_blank"}.

- 確定已設定您的稅捐設定。 另請參閱 [Amazon：稅務政策](https://sellercentral.amazon.com/gp/help/external/help.html){target="_blank"} （需要使用Seller Central登入）。

- 請確定您的送貨方式已正確設定。 若要設定符合下列條件的送貨方法： [!DNL Commerce] 提供給客戶以履行您的Amazon訂單，更新 [Amazon：送貨設定](https://sellercentral.amazon.com/sbr/ref=xx_shipset_dnav_xx#shipping_templates){target="_blank"} 在您的 [!DNL Amazon Seller Central] 帳戶。

## 4.確定已為商店設定您的VAT

（主要由英國賣家使用。） Amazon建議註冊 [Amazon VAT計算服務](https://sell.amazon.co.uk/learn/vat-resources#vat-services-on-amazon){target="_blank"}. 若您選擇不同的方式，則您需負責VAT規定。

>[!NOTE]
>
>Amazon可能需要10到14天的時間來驗證及啟用您的VAT計算服務帳戶。

## 5.增加自動目錄相符專案的數量

在上線期間，Amazon銷售管道會使用產品屬性，將您現有的Amazon清單（如果適用）與您的現有產品比對 [!DNL Commerce] 目錄。 上線後，這些產品屬性會用於發佈您的 [!DNL Commerce] 將目錄專案新增至Amazon清單，以及在此之間同步處理您的產品資料 [!DNL Commerce] 和Amazon。

若要擁有最高數量的 [!DNL Commerce] 產品會自動符合Amazon清單，您應該為您的建立一組產品屬性， [!DNL Commerce] 目錄。 設定Amazon銷售管道商店之前，您應先新增 [!DNL Commerce] 產品屬性以符合這些Amazon屬性，例如：ASIN、EAN、ISBN、UPC或GCID。 另請參閱 [在中建立產品屬性 [!DNL Commerce]](./ob-creating-magento-attributes.md).

## 6.視需要設定貨幣和轉換

如果您的Amazon商店使用與針對設定不同的貨幣 [!DNL Commerce] 商店， [啟用貨幣](https://experienceleague.adobe.com/docs/commerce-admin/config/general/currency-setup.html) 並設定 [貨幣轉換率](https://experienceleague.adobe.com/docs/commerce-admin/stores-sales/site-store/currency/currency-update.html).

## 7.建立產品條件屬性（視需要）

如果您的Amazon清單包含多個產品條件(例如 _新_， _已使用_，或 _喜歡新的_)，建立 [!DNL Commerce] 屬性和指派條件值。 上線期間，您必須將此屬性對應至Amazon條件產品屬性。 另請參閱 [建立Amazon的屬性](./ob-creating-magento-attributes.md).

## 8.設定您的 [!DNL Amazon Seller Central] 送貨方法

若要設定您要提供的送貨方式，以完成Amazon訂單，請參閱 _設定和送貨設定_ 在您的 [!DNL Amazon Seller Central] 帳戶。

## 其他設定

當您的Amazon帳戶設定並作用中時，會有數個 [!DNL Commerce] 有助於簡化Amazon銷售管道上線流程的建議。

### 檢閱並記下您要排除的任何產品

您可能不希望某些產品列在Amazon上。 Amazon sales channel有一個清單規則引擎，用來判斷哪些產品符合發佈至Amazon的資格。 [清單規則](./listing-rules.md) 可讓您選取要發佈（或未發佈）至您的產品的子集。 [!DNL Amazon Seller Central] 帳戶，例如依類別選取或定義一或多個產品屬性。 按讚 [!DNL Commerce] [目錄](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/catalog-rules/price-rules-catalog.html) 或 [購物車](https://experienceleague.adobe.com/docs/commerce-admin/marketing/promotions/cart-rules/price-rules-cart.html) 價格規則，用於Amazon清單資格的產品屬性必須具備 **[!UICONTROL Use for Promo Rule Conditions]** 設為 `Yes`. 請參閱 **[!UICONTROL Use for Promo Rule Conditions]** 在 [產品屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html).

### 設定您的 [!DNL Amazon Seller Central] 區域移至非使用中

為協助在整合期間進行順暢的資料轉換，建議您將Amazon區域設為 `Inactive` 在「設定>帳戶資訊>休假設定」中的狀態。 完成設定後，將狀態變更回 `Active` 在Amazon中。

![「下一步」圖示](assets/btn-next.png) [**繼續建立 [!DNL Commerce] 屬性**](./ob-creating-magento-attributes.md)
