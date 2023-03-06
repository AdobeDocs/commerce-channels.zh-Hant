---
title: 順序設定
description: 使用訂單設定來判斷Amazon訂單如何匯入至您的商務商店及處理。
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: b63e2cfb9c7ba7cc169a6eec954abe782d112c6f
workflow-type: tm+mt
source-wordcount: '1377'
ht-degree: 0%

---

# 順序設定

訂單設定會定義Amazon訂單是否匯入及處理方式 [!DNL Commerce] 可在 [儲存儀表板](./amazon-store-dashboard.md).

訂單匯入設定設為 `Enabled` 依預設，這表示您的Amazon訂單會顯示在存放區控制面板上，並建立對應的 [!DNL Commerce] 訂購。 您可以在 [!DNL Commerce] [訂購](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流程。

>[!NOTE]
>
>無論您的訂單設定為何，在您的商店整合之前存在的Amazon訂單都不會匯入。

之後 [商店整合](./store-integration.md) 完成後，您可以變更訂單設定。 如果您將訂單設定設定為 `Disabled`,Amazon訂單會顯示在商店控制面板上，但必須在您的 [!DNL Amazon Seller Central] 帳戶。

在Amazon上建立訂單時，不會立即匯入至 [!DNL Commerce]. Amazon會指派 `Pending` 狀態為新建立的訂單。 在Amazon驗證訂單和付款方法後，訂單的狀態會變更為 `Unshipped`. 此狀態變更會觸發訂單匯入，而 [!DNL Commerce] 建立相符的對應順序。

從Amazon匯入的訂單可在 [!DNL Commerce] [訂購工作流](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"}. 另請參閱 [管理訂單](./managing-orders.md).

## 配置訂單設定 {#configure-order-settings}

1. 按一下 **[!UICONTROL Order Settings]** 在商店控制面板上。

1. 針對 **[!UICONTROL Import Amazon Orders]** （必要），選擇選項：

   - `Disabled`  — 選擇您不想在 [!DNL Commerce] 從Amazon收到新訂單時。 選擇此選項後，此頁上的所有其他欄位都將被禁用。

   - `Enabled`  — （預設）選擇要建立對應的時間 [!DNL Commerce] 從Amazon收到新訂單時發出的訂單。 [!DNL Commerce] 系統會根據Amazon狀態和庫存層級建立訂單。

      >[!NOTE]
      >
      >匯入Amazon訂單必須設為 `Enabled` 若要管理Amazon訂單，請在 [!DNL Commerce] [訂購](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作流程。 設為時 `Disabled`，您的Amazon訂單沒有對應的 [!DNL Commerce] 訂單編號，無法在 [!DNL Commerce]. 您可以在 [!DNL Amazon Seller Central] 帳戶。

1. 針對 **[!UICONTROL Import Amazon Orders Into Magento Store]**，選擇 [!DNL Commerce] 儲存在中建立對應訂單時，與相關聯的Amazon訂單 [!DNL Commerce].

   此設定預設為當您 [新增Amazon商店](./store-integration.md). 如果要更改此設定，選項清單取決於 [!DNL Commerce] 儲存您已在設定中設定。 請參閱 [商店](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){target="_blank"}.

1. 針對 **[!UICONTROL Customer Creation]**，選擇選項：

   - `No Customer Creation (guest)`  — （預設）選擇您不想在中建立客戶帳戶的時機 [!DNL Commerce] 使用從Amazon訂單匯入的客戶資料。 選擇後， [!DNL Commerce] 處理匯入的Amazon訂單，與處理來賓結帳的方式相同。 [!DNL Commerce].

   - `Build New Customer Account`  — 選擇何時要在 [!DNL Commerce] 使用隨Amazon訂單匯入的客戶資料。 此選項可協助您從Amazon訂單建立客戶資料庫。

1. 針對 **[!UICONTROL Order Number Source]**，選擇選項：

   - `Build Using Magento Order Number`  — （預設）選擇要建立唯一的時間 [!DNL Commerce] 對應Amazon訂單的訂單號碼，使用 [!DNL Commerce] 以增量方式分配訂單ID。

   - `Build Using Amazon Order Number`  — 選擇建立 [!DNL Commerce] 訂單編號，使用相應的Amazon指派訂單編號。
   >[!NOTE]
   >
   >匯入訂單後，Amazon訂單編號會顯示在 _[!UICONTROL Recent Orders]_清單。 此 [!DNL Commerce] 訂單編號顯示於 [!DNL Commerce] [訂購](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} 工作區。

1. 針對 **[!UICONTROL Order Status]** （必要），選擇選項：

   - `Default Order Status`  — （預設）選擇何時要將從Amazon導入的新建立訂單分配給新訂單的定義預設訂單狀態。 新訂單的預設狀態（除非您已為新訂單建立自訂訂單狀態）為 `Pending`. 請參閱 [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html){target="_blank"}.

   - `Custom Order Status`  — 選擇何時要將從Amazon導入的新建立的訂單分配給預設狀態以外的狀態。

   - `Processing Order Status`  — 在 **[!UICONTROL Order Status]** 設為 `Custom Order Status`. 選擇您要用於從Amazon匯入的新建立訂單的狀態。 此欄位中的選項是根據 [!DNL Commerce]. 請參閱 [訂單狀態](https://docs.magento.com/user-guide/sales/order-status.html). 您也可以建立自訂順序狀態，以便在此顯示以供選取。 若要建立自訂訂單狀態，請參閱 [自訂訂單狀態](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}.

1. 完成後，按一下 **[!UICONTROL Save order settings]**.

![順序設定](assets/amazon-order-settings.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Import Amazon Orders] | 選項：<ul><li>**[!UICONTROL Disabled]**  — 選擇您不想在 [!DNL Commerce] 從Amazon收到新訂單時。 選擇此選項後，此頁上的所有其他欄位都將被禁用。</li><li>**[!UICONTROL Enabled]**  — （預設）選擇要建立對應的時間 [!DNL Commerce] 從Amazon收到新訂單時發出的訂單。 [!DNL Commerce] 系統會根據Amazon狀態和庫存層級建立訂單。</li></ul><br><br>`Enabled` 必須選擇在中管理Amazon訂單 [!DNL Commerce]. 當 `Disabled` 選擇後，您的Amazon訂單會顯示在商店控制面板上，但您必須在 [!DNL Amazon Seller Central] 帳戶。 |
| [!UICONTROL Import Amazon Orders Into Magento Store] | 選擇 [!DNL Commerce] 儲存在中建立Amazon訂單時，與相關聯的 [!DNL Commerce] [訂購](https://docs.magento.com/user-guide/sales/orders.html){target="_blank"} workspace. This setting defaults to the Store View for the [!DNL Commerce] website selected when you [added the Amazon store](./store-integration.md). If you want to change this setting, the list of options depends on the [!DNL Commerce] stores you have set up in your configuration. See [Stores](https://docs.magento.com/user-guide/stores/stores-all-stores.html){target="_blank"}. |
| [!UICONTROL Customer Creation] | 選項：<ul><li>**[!UICONTROL No Customer Creation (guest)]**  — （預設）選擇您不想在中建立客戶帳戶的時機 [!DNL Commerce] 使用從Amazon訂單匯入的客戶資料。 選取時，此選項會告訴 [!DNL Commerce] 若要處理匯入的Amazon訂單，其處理來賓結帳的方式與此相同。</li><li>**[!UICONTROL Build New Customer Account]**  — 選擇您要在 [!DNL Commerce] 客戶資料庫，使用隨Amazon訂單匯入的客戶資料。 此選項可協助您建置 [!DNL Commerce] 客戶資料庫。</li></ul> |
| 訂單編號來源 | 選項：<ul><li>**[!UICONTROL Build Using Magento Order Number]**  — （預設）選擇要建立唯一的時間 [!DNL Commerce] 對應Amazon訂單的訂單號碼，使用 [!DNL Commerce] 以增量方式分配訂單ID。 </li><li>**使用Amazon訂單編號建置**  — 選擇建立 [!DNL Commerce] 訂單編號，使用相應的Amazon指派訂單編號。</li></ul> |
| 待定訂單 | 選項：<ul><li>**[!UICONTROL Do Not Reserve Quantity]**  — 選擇您不想要的 [!DNL Commerce] 受您的Amazon訂單影響的庫存數量。 選擇是否將Amazon用於履行流程(FBA)。 當您選擇並收到Amazon訂單時，訂購數量不會影響您的 [!DNL Commerce] 庫存數量。</li><li>**[!UICONTROL Reserve Quantity]**  — 選擇何時要將Amazon訂單中的訂單數量「保留」在 [!DNL Commerce] 庫存數量。 當您選擇並收到Amazon訂單時，訂購數量將「保留」 [!DNL Commerce] 庫存量，以防止您 [!DNL Commerce] 「過賣」的股票。 「保留」數量無法透過 [!DNL Commerce] 店面。</li></ul> |
| [!UICONTROL Order Status] | 選項：<ul><li>**[!UICONTROL Default Order Status]**  — （預設）選擇何時要將從Amazon導入的新建立訂單分配給新訂單的預設訂單狀態。 新訂單的預設狀態（除非您已為新訂單建立自訂訂單狀態）為 `Pending`. 請參閱 [處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html).</li><li>>**[!UICONTROL Custom Order Status]**  — 選擇何時要將從Amazon導入的新建立的訂單分配給預設狀態以外的狀態。 選擇後， **[!UICONTROL Processing Order Status]** 可讓您選擇要用於從Amazon匯入之新建立訂單的狀態。</li></ul> |
| [!UICONTROL Processing Orders Status] | 啟用時機 _[!UICONTROL Order Status]_設為 `Custom Order Status`. 選擇要分配給新訂單的訂單狀態。 此欄位中的選項取決於 [!DNL Commerce]. 請參閱 [訂單狀態](https://docs.magento.com/user-guide/sales/order-status.html){target="_blank"}. You can also create a custom order status to show here. To create a custom order status, see [Custom Order Status](https://docs.magento.com/user-guide/sales/order-status-custom.html){target="_blank"}. |

## [!DNL Commerce] 訂單建立

[!DNL Commerce] 系統會根據下列狀態和庫存條件，為Amazon訂單建立訂單。

### 使用Inventory management建立訂單

>[!NOTE]
>
>僅支援Adobe Commerce和Magento Open Source2.3.x整合。

| 履行管道 | [!DNL Commerce] 庫存狀態 | Amazon訂單狀態 | [!UICONTROL Create Magento Order] 設定 | 庫存預留 |
|---|---|---|---|---|
| FBA | 現車<br>無存貨<br>不管理 | 待定 | 否 | 否 |
| FBA | 現車<br>無存貨<br>不管理 | 待定可用性 | 否 | 否 |
| FBA | 現車<br>無存貨<br>不管理 | 已取消 | 否 | 否 |
| FBA | 現車<br>無存貨<br>不管理 | 錯誤 | 否 | 否 |
| FBA | 現車<br>無存貨<br>不管理 | 未裝運 | 否 | 否 |
| FBA | 現車<br>無存貨<br>不管理 | 部分已發運 | 否 | 否 |
| FBA | 現車<br>不管理 | 已發運 | 是 | 否 |
| FBA | 無存貨 | 已發運 | 否 | 否 |
| FBM | 現車<br>無存貨<br>不管理 | 待定 | 否 | 否 |
| FBM | 現車<br>無存貨<br>不管理 | 待定可用性 | 否 | 否 |
| FBM | 現車<br>無存貨<br>不管理 | 已取消 | 否 | 否 |
| FBM | 現車<br>無存貨<br>不管理 | 錯誤 | 否 | 否 |
| FBM | 現車<br>不管理 | 未裝運 | 是 | 是 |
| FBM | 無存貨 | 未裝運 | 否 | 否 |
| FBM | 現車<br>不管理 | 部分已發運 | 是 | 是 |
| FBM | 無存貨 | 部分已發運 | 否 | 否 |
| FBM | 現車<br>不管理 | 已發運 | 是 | 是 |
| FBM | 無存貨 | 已發運 | 否 | 否 |

>[!NOTE]
>如果Amazon訂單匯入 `Partially Shipped` 或 `Shipped` 狀態，則建立的庫存保留適用於訂單中的所有物料。 Amazon銷售管道不會補償先前出貨的項目。
>
>如果訂單由Amazon(FBA)履行，但物料位於 `out of stock` 狀態， [!DNL Commerce] 無法建立對應的順序。 這是Inventory management整合的限制。
