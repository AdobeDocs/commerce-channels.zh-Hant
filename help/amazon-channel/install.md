---
title: 「安裝 [!DNL Amazon Sales Channel] 擴充功能」
description: 若要整合您的 [!DNL Commerce] 目錄與 [!DNL Amazon Seller Accounts] 並透過 [!DNL Amazon Marketplace]，下載並安裝AmazonSales Channel擴充功能。
role: Admin, Developer
feature: Sales Channels, Install, Integration, Tools and External Services
source-git-commit: 801d4eee9e84b5c5f8b53397fbe8023ad54281e6
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 安裝 [!DNL Amazon Sales Channel] 副檔名

>[!IMPORTANT]
>
>僅限 [!DNL Amazon Sales Channel] Adobe Commerce和Magento Open Source 2.4.x版本支援擴充功能4.0+版本。 如果您執行2.3.x版，請參閱檔案 [相容的Amazon銷售管道版本](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html). 如需版本相容性的詳細資訊，請參閱 [可用性](https://experienceleague.adobe.com/docs/commerce-operations/release/product-availability.html) 開發人員的檔案。

此 [!UICONTROL Amazon Sales Channel] 擴充功能會安裝並新增功能，以將您的Commerce目錄與整合 [!DNL Amazon Seller Accounts] 以透過 [!DNL Amazon Marketplace]. 若要檢閱其他資訊，請參閱 [AmazonSales Channel](https://marketplace.magento.com/magento-module-amazon.html) 頁面位置 [!DNL Commerce Marketplace] 和 [發行說明](release-notes.md).

## 需求

- **商務執行個體**：此 [!DNL Amazon Sales Channel] 擴充功能可安裝在雲端基礎結構2.3.x版或更新版本上具有Magento Open Source、Adobe Commerce和Adobe Commerce的執行個體上。 2.1、2.2或1.x版不再支援。
- **Commerce網頁帳戶**：您應具有Commerce網頁帳戶，用於建立和追蹤API金鑰。
- **API金鑰**：透過您的Commerce網頁帳戶建立Amazon銷售管道API金鑰。 下列指示包含這些步驟。

## 安裝

如需有關在此程式中使用撰寫器的詳細資訊，請參閱 [擴充功能安裝](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) 開發人員檔案中的指示。

1. 登入 [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. 按一下 **[!UICONTROL Marketplace]** 標籤，然後按一下 **[!UICONTROL My Purchases]**.

1. 尋找並選取 **[!UICONTROL Amazon Sales Channel]**.

1. 在擴充功能頁面上，選取版本。

1. 如需元件名稱和版本，請按一下 **[!UICONTROL Technical Details]**.

1. 使用名稱和版本資訊來更新您的中的服務聯結器專案 `composer.json` 檔案。

   - 將擴充功能名稱和版本新增至 `composer.json` 檔案。

   - 導覽至 [!DNL Commerce] 專案目錄並更新 `composer.json` 檔案。

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 輸入您的 [驗證金鑰](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/prerequisites/authentication-keys.html). 您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

   - 請等待Composer完成更新您的專案相依性，並確保沒有錯誤。

1. [驗證擴充功能](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html).

## 新增Amazon sales channel API金鑰

安裝後，輸入 [API金鑰](./amazon-verify-api-key.md) 以完成設定。

## 設定Amazon通道設定選項

您有以下選項可設定Amazon銷售管道。 您不需要修改這些設定，即可開始在Amazon上線和銷售。 建議進階管理員考慮這些選項。

1. 登入Admin。

1. 在 _管理員_ 側欄，前往 **商店** > _設定_ > **設定**.

1. 按一下 **Sales Channel**，然後 **全域設定**.

1. 的 **清除記錄歷史記錄**，定義清除收集記錄檔的間隔。

   選項包括 `Once Daily`， `Once Weekly`、和 `Once Monthly` （預設）。

1. （選用） For **背景工作(CRON)來源**，將設定變更為 `Command Line (CLI) CRON`.

   建議將此設定用於 **_進階使用者/管理員_**.

1. 按一下 **[!UICONTROL Save Config]**.

## 更新擴充功能

1. 登入 [Commerce Marketplace](https://marketplace.magento.com/customer/account/).

1. 按一下 **[!UICONTROL Marketplace]** 標籤，然後按一下 **[!UICONTROL My Purchases]**.

1. 尋找並選取 **[!UICONTROL Amazon Sales Channel]**.

1. 在擴充功能頁面上，選取版本。

1. 如需元件名稱和版本，請按一下 **[!UICONTROL Technical Details]**.

1. 完成 [擴充功能升級指示](https://experienceleague.adobe.com/docs/commerce-operations/installation-guide/tutorials/extensions.html) 在 _安裝指南_.
