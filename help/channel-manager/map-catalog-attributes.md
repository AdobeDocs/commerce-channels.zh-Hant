---
title: 對應目錄屬性
description: '''對應屬性以符合[DNL！ Commerce]產品到現有的 [!DNL Walmart Marketplace] 清單，並在 [!DNL Channel Manager] 和 [!DNL Walmart]之間同步資料。'
feature: Sales Channels, Merchandising, Products
exl-id: 6678d81f-d167-460d-b656-d082d56f670c
source-git-commit: 4670e9b25a840f86862c9cadaf9e6d3e70330b7d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 對應目錄屬性

在從[!DNL Commerce]連結清單到[!DNL Walmart Marketplace]之前，您必須從[!DNL Commerce]目錄至少對應一個唯一識別碼，以對應到Walmart的對應識別碼。

必須執行此步驟才能比對[!DNL Commerce]產品與現有[!DNL Walmart]清單，以及同步處理[!DNL Commerce]與[!DNL Walmart]之間的產品資料。 [!DNL Commerce]產品必須至少有一個產品屬性符合[!DNL Walmart]所需的下列其中一個產品識別碼（產品ID）。

**必要的[!DNL Walmart]產品識別碼**

| **接受的型別** | **名稱** | **用途** | **可接受的位數** |
|-------------------|--------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|
| GTIN | 全球貿易專案 | 一般用途，全球使用 | 14位數 |
| ISBN | 國際標準書號 | 平裝本、精裝本及電子書 | 10或13位數 |
| ISSN | 國際標準序號 | 8位數的序號，用於識別所有媒體印刷和電子媒體上傳送的各種雜誌、期刊、報章和期刊 | 8位數 |
| UPC | 通用產品代碼 | 標準零售追蹤代碼 | 12位數 |

如果您的目錄沒有相符的屬性，請[新增或轉換現有的目錄屬性](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)。

## 對應唯一識別碼

1. 從銷售管道商店的&#x200B;**[!UICONTROL Listings]**&#x200B;或&#x200B;**[!UICONTROL Orders]**&#x200B;頁面，選取&#x200B;**[!UICONTROL Channel Settings]**。

1. 在&#x200B;**[!UICONTROL Channel Settings]**&#x200B;上，選取&#x200B;**[!UICONTROL Map Attributes]**。

   - 尋找要對應的[!DNL Walmart Marketplace]屬性。

   - 從[!DNL Commerce]存放區目錄中選取對應的屬性。

     下列範例將[!UICONTROL Walmart Marketplace UPC]屬性對應至產品目錄中的UPC屬性。

     ![對應產品符合條件的屬性](assets/products-map-attributes-for-match.png){width="600" zoomable="yes"}

   - 選取&#x200B;**[!UICONTROL Save]**。
