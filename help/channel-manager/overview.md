---
title: '"簡介 [!DNL Channel Manager]"'
description: 瞭解如何安裝和使用 [!DNL Channel Manager] 將Adobe Commerce和Magento Open Source商店與第三方市場整合，並建立銷售渠道，從您的商務管理員無縫地管理市場清單、定價、庫存和銷售。
role: User
level: Intermediate
source-git-commit: ff87f31fec7a689385a93b8cab260fd93ff15f90
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---


# 概述

Adobe Commerce和Magento Open Source的渠道經理在管理員中提供了一個方便的工作區，以管理第三方市場(如沃爾瑪、Amazon和eBay)上的渠道銷售。 增加銷售並擴展到新市場，同時從您的商務管理員無縫管理銷售渠道運營。

![[!DNL Channel Manager] 擴展管理員視圖](assets/channel-manager-admin-entry-page.png)

## Beta版本概述

渠道經理的Beta版本支援希望在沃爾瑪市場上提供產品的Adobe Commerce或Magento Open Source銷售商。

此版本支援以下管理銷售渠道操作的功能：

* 在Adobe Commerce或Magento Open Source與沃爾瑪市場之間建立API連接

* 使用產品匹配將產品從渠道經理發布到沃爾瑪

* 在Channel Manager中查看產品清單狀態，例如 *草案*。 *處理*。 *匹配*。 *錯誤*。

* 同步從Commerce到Walmart的匹配產品的庫存數量

* 從Commerce到Walmart的匹配產品同步目錄定價

* 從Walmart Marketplace接收訂單，並在 [!DNL Commerce] 訂單面板

### Channel Manager操作的預期延遲

資料同步過程 [!DNL Channel Manager] 和連結 [!DNL Walmart Marketplace] 商店需要一些時間才能完成。 查看的預期處理時間 [!DNL Channel Manager] 操作以幫助計畫銷售渠道運營工作。

**Channel Manager操作的估計延遲**
| **操作**                              | **說明**                                                                                                                               | **預期延遲**                                                                                                        | |—|—| |將產品添加到Channel Manager |從Commerce產品目錄中選擇產品，然後將其導入Channel Manager。                                                       | **最多5分鐘** — 如果您選擇了許多產品，例如，整個產品目錄，則導入過程需要更長時間。 | |在沃爾瑪市場上匹配產品 |在渠道經理中選擇產品清單，然後發送到沃爾瑪進行匹配。                                                                  | **最多30分鐘** — 如果選擇了多個產品，則匹配過程將花費更長的時間，具體取決於選定的數量。   | |清單更新 | Commerce中庫存數量更改時。 渠道經理將更新同步到Walmart。                                                         | **最多10分鐘**                                                                                                      | |價格更新 |當產品價格發生變化時，渠道經理會將更新同步到Walmart。                                                                    | **最多5分鐘**                                                                                                       | |從Walmart到Commerce的訂單同步 |客戶在沃爾瑪市場上訂購商務產品。 沃爾瑪將訂單發給渠道經理。 訂單按訂單儀表板顯示。 | **最多30分鐘**                                                                                                      | |在Oracle Commerce Order Management中建立的訂單 |渠道經理從Walmart訂單建立Commerce訂單，並更新訂單控制面板以包括Commerce訂單編號。       | **最多5分鐘**                                                                                                       |

## 沃爾瑪先決條件

您需要從沃爾瑪獲得以下資訊才能將Commerce與Walmart Marketplace整合：

* 批准在沃爾瑪上銷售和登錄註冊的Marketplace Seller帳戶的憑據

* 將Adobe Commerce或Magento Open Source連接到Walmart Marketplace的API密鑰

   Walmart Marketplace API密鑰支援Adobe Commerce或Magento Open Source的渠道經理與Walmart Marketplace之間的整合。 在啟動Channel Manager登錄過程之前，在Seller Central中設定API密鑰。

### 設定Marketplace賣家帳戶

1. [提交您的沃爾瑪銷售商申請](https://marketplace-apply.walmart.com/apply?id=0014M00001zivMpQAI)
2. 在獲得沃爾瑪批准後， [設定沃爾瑪賣家帳戶](https://sellerhelp.walmart.com/seller/s/guide?article=000008219)。

### 生成Walmart Marketplace API密鑰

1. 轉到Walmart Marketplace以生成 [解決方案提供商生產API密鑰，用於Adobe](https://developer.walmart.com/#preloginModal?redirectUri=https%3A%2F%2Fdeveloper.walmart.com%2Faccount%2FgenerateKey)。

1. 建立密鑰並配置權限：

   * 選擇「Adobe」作為解決方案提供商。

   * 如下表所示設定權限。 有關詳細資訊，請參閱 [API憑據](https://sellerhelp.walmart.com/seller/s/guide?article=000006422) 的 _沃爾瑪市場銷售商幫助_。

|    **AdobeAPI鍵配置**
| **權限** | **設定** | |—| |內容 |完全訪問 | |獲取源 |僅查看 | |清單 |完全訪問 | |項 |完全訪問 | |延遲時間 |完全訪問 | |順序 |完全訪問 | |價格 |完全訪問 | |報告 |僅查看 | |返回 |完全訪問 | |規則 |完全訪問 | |裝運 |完全訪問 |

## Walmart Marketplace商店狀態

當您向沃爾瑪市場發佈產品時，列出產品的可用性取決於您的沃爾瑪市場商店的狀態：

* 對於現場商店，在匹配操作完成後，您的產品優惠即會列出並可供銷售。

* 對於不即時的商店，您的產品優惠將被提供，而且客戶無法看到。 一旦該商店開始上線，就會自動將臨時的清單推送到現場商店。


![[!DNL Walmart Seller Central] 分段產品](assets/walmart-seller-central-staged.png)
