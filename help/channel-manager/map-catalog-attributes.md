---
title: 映射目錄屬性
description: 映射匹配的屬性[DNL! Commerce]產品到現有 [!DNL Walmart Marketplace] 清單和同步資料 [!DNL Channel Manager] 和 [!DNL Walmart]。
source-git-commit: dfe56db25bb569ad70fb1036d539797bbb126dd5
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# 映射目錄屬性

在發佈來自 [!DNL Commerce] 至 [!DNL Walmart Marketplace]，必須從 [!DNL Commerce] 從Walmart獲取相應標識符。
需要此步驟才能匹配 [!DNL Commerce] 現有產品 [!DNL Walmart] 清單和同步產品資料 [!DNL Commerce] 和 [!DNL Walmart]。

對於產品匹配，Commerce產品必須至少有一個產品屬性與以下產品標識符（產品ID）之一匹配， [!DNL Walmart]。

**需要的Walmart產品ID**

| **接受類型** | **名稱** | **目的** | **可接受數字** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| 格丁 | 全球貿易項目 | 一般用途，全球使用 | 14位 |
| ISBN | 國際標準書號 | 平裝書、精裝書和電子書 | 10或13位 |
| ISSN | 國際標準序列號 | 8位序列號，用於識別所有媒體印刷和電子出版物上的各類雜誌、期刊、報紙和期刊 | 8位 |
| UPC | 通用產品代碼 | 標準零售跟蹤代碼 | 12位 |

如果目錄沒有與其中一種類型匹配的屬性， [添加或轉換現有目錄屬性](https://docs.magento.com/user-guide/catalog/product-attributes.html)。

## 映射唯一標識符

1. 在 [!UICONTROL Listings] 頁，選擇 **[!UICONTROL Settings]**。

   - 查找要映射的Walmart Marketplace屬性。

   - 從 [!DNL Commerce] 儲存目錄。

      以下示例將Walmart Marketplace UPC屬性映射到產品目錄中的UPC屬性。
   ![映射產品匹配條件的屬性](assets/products-map-attributes-for-match.png)

   - 選擇 **[!UICONTROL Save]**。


## 更新映射的屬性配置

通過更新映射的屬性設定來更改匹配產品的Commerce產品標識符。

例如，您可以根據SKU進行匹配，而不是基於Commerce UPC產品屬性代碼進行匹配。 或者，映射其他屬性以改進匹配。

1. 從 **[!UICONTROL Listings]**&#x200B;選中 **[!UICONTROL Settings]**。

1. 在「映射」屬性窗體中，根據需要更改映射的屬性配置。
