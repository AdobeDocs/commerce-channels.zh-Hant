---
title: 映射目錄屬性
description: '映射匹配的屬性[DNL! Commerce]產品轉換至現有 [!DNL Walmart Marketplace] 清單和同步資料 [!DNL Channel Manager] 和 [!DNL Walmart].'
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: aeeaca20cb54528f77e457d54a194d6603c08654
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 映射目錄屬性

在您從 [!DNL Commerce] to [!DNL Walmart Marketplace]，您必須從 [!DNL Commerce] 從沃爾瑪目錄到相應的標識符。

必須執行此步驟才能符合 [!DNL Commerce] 產品至現有 [!DNL Walmart] 清單和同步產品資料 [!DNL Commerce] 和 [!DNL Walmart]. 此 [!DNL Commerce] 產品必須至少有一個產品屬性，符合下列產品識別碼（產品ID）之一， [!DNL Walmart].

**必填 [!DNL Walmart] 產品ID**

| **接受類型** | **名稱** | **用途** | **可接受位數** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | 全球貿易項目 | 一般用途，全球使用 | 14位數 |
| ISBN | 國際標準書號 | 平裝書、硬套和電子書 | 10或13位數 |
| ISSN | 國際標準序列號 | 8位序列號，用於識別所有媒體印刷品和電子印刷品上的各類雜誌、期刊、報紙和期刊 | 8位數 |
| UPC | 通用產品代碼 | 標準零售追蹤代碼 | 12位數 |

如果目錄沒有相符的屬性， [新增或轉換現有目錄屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html).

## 映射唯一標識符

1. 從 **[!UICONTROL Listings]** 或 **[!UICONTROL Orders]** 頁面，請選取 **[!UICONTROL Channel Settings]**.

1. 開啟 **[!UICONTROL Channel Settings]**，選取 **[!UICONTROL Map Attributes]**.

   - 尋找 [!DNL Walmart Marketplace] 屬性來對應。

   - 從 [!DNL Commerce] 儲存目錄。

      下列範例將 [!UICONTROL Walmart Marketplace UPC] 屬性至產品目錄中的UPC屬性。

      ![對應產品符合條件的屬性](assets/products-map-attributes-for-match.png)

   - 選擇 **[!UICONTROL Save]**.
