---
title: 管理Amazon清單的屬性
description: 您可以管理Commerce產品屬性與Amazon屬性的對應，以確保系統之間的產品資訊準確。
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 管理Amazon清單的屬性

Amazon和 [!DNL Commerce] 兩者都使用用於定義產品的產品屬性系統（稱為屬性）。 屬性可定義產品的說明、內容、影像、價格及各種資料。

Commerce和Amazon之間的成功通訊需要 [!DNL Commerce] 屬性必須正確對應（或比對）至對應的Amazon屬性。 與Amazon整合時，您可以將這些屬性對應至Amazon屬性。 完成時， [!DNL Commerce] 可與您的同步並維護您的Amazon清單 [!DNL Commerce] 產品目錄。

例如，想像您有相同專案在 [!DNL Commerce] 目錄和Amazon清單。 產品的一個屬性可能是料號的清單價格。 中的上市價格名稱 [!DNL Commerce] 可命名為 `Price`，而Amazon的掛牌價格可能會命名為 `ListingPrice`. 您必須指示 [!DNL Commerce] 在與Amazon通訊時， [!DNL Commerce] 已命名的屬性 `Price` 與命名的Amazon屬性相同 `ListingPrice`. 此程式稱為 _管理屬性_，包括建立和編輯現有屬性。 確定屬性已正確比對，確保兩者之間的通訊正確 [!DNL Commerce] 和Amazon。

設定屬性對應時， [!DNL Commerce] 可與Amazon來回溝通產品資訊。 如果您有Amazon產品清單， [!DNL Commerce] 可以將您的Amazon產品和詳細資料匯入 [!DNL Commerce] 目錄，可讓您從單一集中式產品目錄管理您的Amazon清單。

Amazon sales channel可讓您視需要存取、檢閱、建立和管理屬性，於 [_[!UICONTROL Attributes]_檢視](./attributes-view.md) ，位於Amazon sales channel首頁。 如果您將屬性新增至 [!DNL Commerce] 型錄，則可能需要更新所有產品的這些值。

有關詳細資訊 [!DNL Commerce] 和Amazon屬性集和值，請參閱：

- [管理屬性基本需知](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [建立屬性](./creating-attributes.md#create-an-attribute)
- [編輯現有屬性](./creating-attributes.md#edit-an-attribute)
- [檢視屬性對應](./amazon-matching-attributes-values.md)
- [編輯或建立屬性對應](./amazon-manually-update-incomplete-listing.md)
