---
title: 管理Amazon清單的屬性
description: 您可以管理Commerce產品屬性與Amazon屬性的對應，以確保系統之間的產品資訊準確無誤。
feature: Sales Channels, Products, Configuration
exl-id: 6f9ded2d-292e-4b7e-8c10-48f478a4383e
source-git-commit: 7fff4c463551089fb64f2d5bf7bf23f272ce4663
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 管理Amazon清單的屬性

Amazon和[!DNL Commerce]都使用用於定義產品的產品屬性系統（稱為屬性）。 屬性可定義產品的說明、內容、影像、價格及各種資料。

Commerce與Amazon之間的成功通訊要求[!DNL Commerce]屬性正確對應（或比對）至對應的Amazon屬性。 與Amazon整合時，您可以將這些屬性對應至Amazon屬性。 完成後，[!DNL Commerce]就可以將您的Amazon清單與您的[!DNL Commerce]產品目錄同步並加以維護。

例如，假設您的[!DNL Commerce]目錄和Amazon清單中有相同專案。 產品的一個屬性可能是料號的清單價格。 在[!DNL Commerce]中的上市價格名稱可能名為`Price`，而Amazon的上市價格可能名為`ListingPrice`。 您必須指示[!DNL Commerce]在與Amazon通訊時，名為`Price`的[!DNL Commerce]屬性與名為`ListingPrice`的Amazon屬性相同。 此程式稱為&#x200B;_管理屬性_，包括建立新屬性和編輯現有屬性。 確定屬性正確相符，以確保[!DNL Commerce]與Amazon之間的正確通訊。

設定屬性對應時，[!DNL Commerce]可以與Amazon來回通訊產品資訊。 如果您有Amazon產品清單，則[!DNL Commerce]可以將您的Amazon產品和詳細資料匯入您的[!DNL Commerce]目錄，讓您從單一集中式產品目錄管理您的Amazon清單。

Amazon sales channel可讓您視需要存取、檢閱、建立及管理Amazon sales channel首頁上&#x200B;[_[!UICONTROL Attributes]_檢視](./attributes-view.md)中的屬性。 如果您將屬性新增至您的[!DNL Commerce]目錄，則可能需要更新所有產品的這些值。

如需[!DNL Commerce]與Amazon屬性集和值的詳細資訊，請參閱：

- [管理屬性基本資訊](https://experienceleague.adobe.com/docs/commerce-admin/catalog/product-attributes/product-attributes.html)
- [建立屬性](./creating-attributes.md#create-an-attribute)
- [編輯現有屬性](./creating-attributes.md#edit-an-attribute)
- [檢視屬性對應](./amazon-matching-attributes-values.md)
- [編輯或建立屬性對應](./amazon-manually-update-incomplete-listing.md)
