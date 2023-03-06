---
title: 商店整合
description: 開始上線程式之前，您必須建立（新增）AmazonSales Channel商店，並將其連線至您的Amazon賣家帳戶。
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 商店整合

若要開始使用Amazon銷售管道，您必須建立（新增）Amazon銷售管道商店，並將其連線至您的Amazon銷售者帳戶。 這兩個步驟整合您的 [!DNL Commerce] 和Amazon帳戶共用資料、同步產品等。

_您需要的主要登入憑證 [!DNL Amazon Seller Central] 帳戶（用來建立賣家帳戶的電子郵件或電話）來連線您的商店。_

>[!NOTE]
>
>首次商店整合後，系統會每年提示您重新授與存取權，以續約Amazon銷售管道與Amazon的連線。 您可以在 _當前授權_ 表格 _Amazon MWS開發人員權限_ 區段 **設定** > **使用者權限** 賣主中心帳戶的頁面。

## 新增Amazon商店

1. 在 _管理_ 邊欄，轉到 **行銷** > _管道_ > **AmazonSales Channel**.

   新增您的第一個Amazon銷售管道商店時， _預先設定任務_ 的上界。 新增第一個商店後，即可在 [Amazon銷售頻道首頁](./amazon-sales-channel-home.md) 頁面底下 _學習與準備_ 的上界。

1. 按一下 **[!UICONTROL Add Amazon Store]**.

   此 _[!UICONTROL Add Amazon sales channel]_頁面開啟。

   ![新增Amazon銷售管道商店](assets/amazon-store-integration.png)

1. 針對 **[!UICONTROL Magento Website to use for Amazon Listing]**，選擇 [!DNL Commerce] 連線至此Amazon銷售渠道商店的網站。

   此設定也會定義預設值 [!DNL Commerce] 儲存 [匯入Amazon訂單](./order-settings.md).

1. 針對 **[!UICONTROL Email Address]**，輸入您慣用的聯絡人電子郵件地址。

1. 針對 **[!UICONTROL New Store Name]**，輸入新Amazon銷售管道商店的描述性名稱。

   >[!NOTE]
   >
   >此名稱會作為 [!DNL Commerce] 僅參考並識別 [Amazon銷售頻道首頁](./amazon-sales-channel-home.md) 頁面。 您希望讓團隊能夠輕鬆識別。 例如，您在美國地區銷售的Amazon商店可能會命名為 `Amazon Store USA`.

1. 針對 **[!UICONTROL Amazon Marketplace Country]**，選擇此Amazon銷售管道商店銷售產品的地區/國家/地區。 選項：

   - 美國
   - 加拿大
   - 墨西哥
   - 英國

1. 在 _[!UICONTROL Map your Magento attributes to Amazon]_部分，請執行以下操作：

   - 針對 **[!UICONTROL Product ID on the Amazon market]**，選擇要對應至的Amazon屬性 [!DNL Commerce] 屬性。

      此ID有助於正確比對您 [!DNL Commerce] 目錄。

   - 針對 **[!UICONTROL Map a Magento attribute]**，選擇 [!DNL Commerce] 產品屬性，以對應至上方選取的Amazon屬性。

      [對應屬性](./ob-creating-magento-attributes.md) 有助於確保Amazon清單正確符合您 [!DNL Commerce] 目錄。

1. 按一下 **[!UICONTROL Connect]**.

   對話框關閉，新商店出現在 [Amazon銷售頻道首頁](./amazon-sales-channel-home.md) 頁面，其中包含確認訊息。

## 將商店連接到 [!DNL Amazon Seller Central]

1. 在商店控制面板上，按一下 **[!UICONTROL Connect store]** 在商店卡上啟動 [!DNL Amazon Seller Central] 的子句。

1. 輸入 [!DNL Amazon Seller Central] 帳戶憑證，按一下 **[!UICONTROL Sign in]**.

   若要完成此連線，您必須登入 [!DNL Amazon Seller Central] 使用主要使用者登入憑證的帳戶（用來建立賣家帳戶的電子郵件或電話）。

1. 如果出現提示，請輸入您從Amazon收到的代碼，然後按一下，以完成Amazon雙因素授權(2FA) **[!UICONTROL Sign in]**.

1. 在 _[!UICONTROL Amazon Marketplace Web Service]_確認頁面，選擇「[!UICONTROL I understand...]「 」核取方塊，按一下&#x200B;**[!UICONTROL Next]**.

1. 在 _[!UICONTROL You are almost done]_訊息，按一下&#x200B;**[!UICONTROL Continue]**.

   您已授予Amazon銷售管道權限，可存取資料並與您的 [!DNL Amazon Seller Central] 帳戶。 Amazon頁面關閉，並顯示確認訊息。

   此 [Amazon銷售頻道首頁](./amazon-sales-channel-home.md) 顯示Amazon商店卡片的頁面隨即開啟。

   若要檢視商店控制面板，請按一下 **[!UICONTROL View Store]** 在商店卡上。

![Amazon銷售渠道首頁，帶有新商店卡](assets/asc-dashboard-after-2fa.png)

您新的Amazon銷售管道商店現已連線至 [!DNL Amazon Seller Central] 帳戶。

![下一個表徵圖](assets/btn-next.png) [**繼續建立清單規則**](./ob-create-listing-rule.md)
