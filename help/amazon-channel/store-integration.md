---
title: 儲存整合
description: 在啟動登機過程之前，必須建立（添加）一個AmazonSales Channel商店並將其連接到您的Amazon賣家帳戶。
exl-id: ea79e91d-7d92-4992-a921-7ac7632a0519
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 儲存整合

要開始使用Amazon銷售渠道，您必須建立（添加）Amazon銷售渠道商店並將其連接到您的Amazon銷售帳戶。 這兩個步驟整合了您 [!DNL Commerce] 和Amazon客戶共用資料、同步產品等。

_您需要主登錄憑據 [!DNL Amazon Seller Central] 帳戶（用於建立賣家帳戶的電子郵件或電話）以連接您的商店。_

>[!NOTE]
>
>在您首次整合商店後，系統將每年提示您重新授予訪問權，以續訂到Amazon的Amazon銷售渠道連接。 您可以在 _當前授權_ 的 _AmazonMWS開發人員權限_ 的下界 **設定** > **用戶權限** 銷售中心帳戶的頁面。

## 添加Amazon商店

1. 在 _管理_ 邊欄，轉到 **營銷** > _頻道_ > **AmazonSales Channel**。

   添加您的第一家Amazon銷售渠道商店時， _預設定任務_ 模式。 添加第一個儲存後，可以在 [Amazon銷售渠道首頁](./amazon-sales-channel-home.md) 頁 _學習和準備_ 的上界。

1. 按一下 **[!UICONTROL Add Amazon Store]**。

   的 _[!UICONTROL Add Amazon sales channel]_的上界。

   ![添加Amazon銷售渠道商店](assets/amazon-store-integration.png)

1. 對於 **[!UICONTROL Magento Website to use for Amazon Listing]**，選擇 [!DNL Commerce] 連接此Amazon銷售渠道商店的網站。

   此設定還定義預設 [!DNL Commerce] 儲存 [導入Amazon訂單](./order-settings.md)。

1. 對於 **[!UICONTROL Email Address]**，輸入首選聯繫人電子郵件地址。

1. 對於 **[!UICONTROL New Store Name]**，輸入新Amazon銷售渠道商店的描述性名稱。

   >[!NOTE]
   >
   >此名稱用作 [!DNL Commerce] 僅引用並標識 [Amazon銷售渠道首頁](./amazon-sales-channel-home.md) 的子菜單。 你希望讓它成為你的團隊能夠輕易識別的東西。 例如，您在美國地區銷售的Amazon商店可能會被命名為 `Amazon Store USA`。

1. 對於 **[!UICONTROL Amazon Marketplace Country]**，選擇此Amazon銷售渠道商店銷售產品的地區/國家/地區。 選項：

   - 美國
   - 加拿大
   - 墨西哥
   - 英國

1. 在 _[!UICONTROL Map your Magento attributes to Amazon]_，請執行以下操作：

   - 對於 **[!UICONTROL Product ID on the Amazon market]**，選擇要映射到 [!DNL Commerce] 屬性。

      此ID有助於正確匹配您的 [!DNL Commerce] 目錄。

   - 對於 **[!UICONTROL Map a Magento attribute]**&#x200B;的子菜單。 [!DNL Commerce] 要映射到上面選擇的Amazon屬性的product屬性。

      [映射屬性](./ob-creating-magento-attributes.md) 有助於確保您的Amazon清單與您的相應產品正確匹配 [!DNL Commerce] 目錄。

1. 按一下 **[!UICONTROL Connect]**。

   對話框關閉，新儲存將出現在 [Amazon銷售渠道首頁](./amazon-sales-channel-home.md) 的子菜單。

## 將儲存連接到 [!DNL Amazon Seller Central]

1. 在儲存儀表板上，按一下 **[!UICONTROL Connect store]** 在要啟動的商店卡上 [!DNL Amazon Seller Central] 的子菜單。

1. 輸入 [!DNL Amazon Seller Central] 帳戶憑據，按一下 **[!UICONTROL Sign in]**。

   要完成此連接，必須登錄到 [!DNL Amazon Seller Central] 使用主用戶的登錄憑據（用於建立賣家帳戶的電子郵件或電話）的帳戶。

1. 如果出現提示，請輸入從Amazon接收的代碼，然後按一下，完成Amazon雙因素授權(2FA) **[!UICONTROL Sign in]**。

1. 在 _[!UICONTROL Amazon Marketplace Web Service]_確認頁，選擇「[!UICONTROL I understand...]&quot;複選框，按一下&#x200B;**[!UICONTROL Next]**。

1. 在 _[!UICONTROL You are almost done]_消息，按一下&#x200B;**[!UICONTROL Continue]**。

   您已授予Amazon銷售渠道權限，可以訪問和共用您的資料 [!DNL Amazon Seller Central] 帳戶。 Amazon頁面關閉，並顯示確認消息。

   的 [Amazon銷售渠道首頁](./amazon-sales-channel-home.md) 開啟，顯示您的Amazon商店卡。

   要查看儲存儀表板，請按一下 **[!UICONTROL View Store]** 在商店卡上。

![Amazon銷售渠道首頁，新店卡](assets/asc-dashboard-after-2fa.png)

您的新Amazon銷售渠道商店現已連接到您 [!DNL Amazon Seller Central] 帳戶。

![下一個表徵圖](assets/btn-next.png) [**繼續建立清單規則**](./ob-create-listing-rule.md)
