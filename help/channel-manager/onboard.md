---
title: 板載 [!DNL Channel Manager]
description: 將實例連接到 [!DNL Channel Manager] 完成幾個單車步驟。
role: User
level: Intermediate
exl-id: 7c4ccd9e-ae32-4511-8d1e-baa690604612
source-git-commit: 30495c4e47f15c821206f7b0252b868b4e27d62d
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# 板載 [!DNL Channel Manager]

通過在上安裝Channel Manager擴展，板載Channel Manager [!DNL Commerce] 實例和配置API連接。 這些連接可在您的Commerce實例和 [!DNL Walmart Marketplace]。

完成登錄後，請通過 [!UICONTROL Channel Manager] 的上界 [!UICONTROL Commerce Admin Marketing] 的子菜單。

![[!DNL Channel Manager] 管理視圖中的選項](assets/channel-manager-admin-view.png)

## 登機概述

1. [安裝 [!DNL Channel Manager] 擴展](install.md)。

1. [配置 [!DNL Commerce Services Connector]](connect.md) 將Channel Manager與Commerce實例和其他支援服務整合。

1. [連接 [!DNL Commerce] 儲存 [!DNL Walmart Marketplace]](connect.md)。

1. [完成商店設定](complete-store-setup.md)。

## 先決條件

- 驗證您是否具有 [沃爾瑪市場先決條件](walmart-prerequisites.md) 與Channel Manager整合。

- **商業帳戶資訊** — 下載和安裝 [!DNL Channel Manager] 需要 [商業帳戶](https://docs.magento.com/user-guide/magento/magento-account.html){target=&quot;_blank&quot;}。 您需要具有「所有者」或「管理員」訪問權限的帳戶ID和憑據 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 實例。

   - **影像ID**-[登錄](https://account.magento.com/customer/account/login/) 到Commerce帳戶以從 **[!UICONTROL My Account - Magento settings]**。 您需要此ID註冊 [!DNL Channel Manager] 服務測試程式。

      ![[!DNL MAGEID] 在商業帳戶設定上](assets/mageid-my-commerce-account.png)

   - **訪問密鑰 —** 獲取身份驗證密鑰以從Commerce Composer儲存庫下載Commerce擴展 `([!DNL repo.magento.com]`)。

      ![[!UICONTROL Commerce Marketplace access keys]](assets/commerce-marketplace-access-keys.png)

      在Adobe Commerce和Magento Open Source項目上，所有者可以 [共用訪問](https://docs.magento.com/user-guide/magento/magento-account-share.html) 允許受信任的員工和服務提供商使用所有者或許可證持有者帳戶的憑據下載擴展。

      對於 [!DNL Adobe Commerce] 在雲基礎架構項目上，軟體安裝程式必須具有以下訪問權限 [!DNL Commerce] 實例：

      - 超級用戶對雲項目的訪問
      - 管理員對特定環境的訪問
      - 一個 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 具有訪問Composer儲存庫權限的帳戶

      請參閱 [管理用戶訪問](https://devdocs.magento.com/cloud/project/user-admin.html)。


- **下載Channel Manager Composer包的授權** — 為Adobe通道提供Beta協調器，其MAGE ID [!DNL Commerce] 用於管理組織服務的帳戶。
- **使用Composer和[!DNL Commerce CLI]**  — 請參閱 [常規CLI安裝](https://devdocs.magento.com/extensions/install/){target=&quot;_blank&quot;，瞭解有關使用這些工具在上安裝和配置擴展的資訊 [!DNL Adobe Commerce] 或 [!DNL Magento Open Source] 平台。
- [[!DNL Amazon Sales Channel] 4.4.2版或更高版本](https://experienceleague.adobe.com/docs/commerce-channels/amazon/release-notes.html) — 如果已激活 [!DNL Amazon Sales Channel] 為 [!DNL Commerce] 站點，驗證 [!DNL Commerce] 平台在安裝之前已安裝4.42版 [!DNL Channel Manager]。

### 要求

- [Adobe Commerce2.4.x](https://devdocs.magento.com/release/released-versions.html)
- [7.3菲律賓比索/7.4](https://devdocs.magento.com/guides/v2.4/install-gde/prereq/php-settings.html)
- [作曲家1.x或更高版本](https://devdocs.magento.com/cloud/reference/cloud-composer.html)


### 支援的平台

- Adobe Commerce雲(ECE):2.4.x
- Adobe Commerce駐地：2.4.x
- Magento Open Source2.4.x
