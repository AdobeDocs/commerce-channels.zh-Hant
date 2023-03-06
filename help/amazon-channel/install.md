---
title: 安裝擴充功能
description: 若要整合您的 [!DNL Commerce] 目錄 [!DNL Amazon Seller Accounts] 然後通過 [!DNL Amazon Marketplace]，下載並安裝AmazonSales Channel擴充功能。
exl-id: ebf22e28-b6a2-420b-80ca-2d750839286c
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 安裝擴充功能

>[!IMPORTANT]
>
>僅 [!DNL Amazon Sales Channel] Adobe Commerce和Magento Open Source2.4.x版支援擴充功能4.0+版。 如果您執行的是2.3.x版，請參閱 [相容的Amazon銷售管道版本](https://docs.magento.com/user-guide/v2.3/sales-channels/amazon/amazon-sales-channel.html){target="_blank"}. For more information about version compatibility, see the [Availability](https://devdocs.magento.com/release/availability.html){target="_blank"} 頁面。

此 [!UICONTROL Amazon Sales Channel] 擴充功能安裝並新增功能，將您的商務目錄與 [!DNL Amazon Seller Accounts] 通過 [!DNL Amazon Marketplace]. 若要檢閱其他資訊，請參閱 [AmazonSales Channel](https://marketplace.magento.com/magento-module-amazon.html) 頁面 [!DNL Commerce Marketplace] 和 [發行說明](release-notes.md).

## 需求

- **商務例項**:此 [!DNL Amazon Sales Channel] 擴充功能可安裝在雲端基礎架構2.3.x版或更新版本上具有Magento Open Source、Adobe Commerce和Adobe Commerce的執行個體上。 2.1、2.2或1.x版不再支援此功能。
- **商務Web帳戶**:您應有Commerce Web帳戶，可用來建立及追蹤API金鑰。
- **API金鑰**:透過您的Commerce網站帳戶建立Amazon銷售管道API金鑰。 下列指示包括這些步驟。

## 安裝

如需有關為此程式使用撰寫器的詳細資訊，請參閱 [擴充功能安裝](https://devdocs.magento.com/extensions/install/){target="_blank"} 開發人員檔案中的指示。

1. 登入 [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. 按一下 **[!UICONTROL Marketplace]** ，然後按一下 **[!UICONTROL My Purchases]**.

1. 尋找並選取 **[!UICONTROL Amazon Sales Channel]**.

1. 在擴充功能頁面上，選取版本。

1. 如需元件名稱和版本，請按一下 **[!UICONTROL Technical Details]**.

1. 使用名稱和版本資訊來更新 `composer.json` 檔案。

   - 將擴充功能的名稱和版本新增至 `composer.json` 檔案。

   - 導覽至 [!DNL Commerce] 專案目錄和更新您的 `composer.json` 檔案。

   ```bash
   composer require magento/services-connector:~1.0.3
   ```

   - 輸入 [驗證金鑰](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/connect-auth.html){target="_blank"}. 您的公開金鑰是您的使用者名稱；您的私密金鑰是您的密碼。

   - 等待撰寫器完成專案相依性的更新，並確保沒有錯誤。


1. [驗證擴充功能](https://devdocs.magento.com/extensions/install/#verify-the-extension){target="_blank"}.

## 新增Amazon銷售管道API金鑰

安裝後，請輸入 [API金鑰](./amazon-verify-api-key.md) 完成配置。

## 設定Amazon通道設定選項

您有下列選項可設定Amazon銷售管道。 您不需要修改這些設定即可開始在Amazon上上線和銷售。 建議進階管理員考慮這些選項。

1. 登入管理員。

1. 在 _管理_ 邊欄，轉到 **商店** > _設定_ > **設定**.

1. 按一下 **Sales Channel**，然後 **全域設定**.

1. 針對 **清除日誌歷史記錄**，定義清除收集記錄檔的間隔。

   選項包括 `Once Daily`, `Once Weekly`，和 `Once Monthly` （預設）。

1. （選用）適用於 **背景任務(CRON)源**，請將設定變更為 `Command Line (CLI) CRON`.

   建議使用此設定 **_進階使用者/管理員_**.

1. 按一下 **[!UICONTROL Save Config]**.

## 更新擴充功能

1. 登入 [Commerce Marketplace](https://marketplace.magento.com/customer/account/){target="_blank"}.

1. 按一下 **[!UICONTROL Marketplace]** ，然後按一下 **[!UICONTROL My Purchases]**.

1. 尋找並選取 **[!UICONTROL Amazon Sales Channel]**.

1. 在擴充功能頁面上，選取版本。

1. 如需元件名稱和版本，請按一下 **[!UICONTROL Technical Details]**.

1. 完成 [擴充功能升級指示](https://devdocs.magento.com/extensions/install/#upgrade-an-extension){target="_blank"} 在開發人員檔案中。
