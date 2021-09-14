---
title: 順序設定
description: 使用訂單設定來判斷Amazon訂單如何匯入至您的商務商店及進行處理。
redirect_from: /sales-channels/asc/ob-order-settings.html
exl-id: dc8d0ce1-86a8-4949-b49a-73c5cf62db16
source-git-commit: 632157839130461869345724bdfc03b306a4f613
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# 順序設定

訂單設定會定義在[!DNL Commerce]中匯入及處理Amazon訂單的方式，以及可在[儲存控制面板](./amazon-store-dashboard.md)上存取的方式。

訂單匯入設定預設會設為`Enabled`，這表示您的Amazon訂單會出現在商店控制面板上，並建立對應的[!DNL Commerce]訂單。 可在[!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}工作流程中管理匯入的訂單。

>[!NOTE]
>
>無論您的訂單設定為何，在您的商店整合之前存在的Amazon訂單都不會匯入。

完成[儲存整合](./store-integration.md)後，您可以變更訂單設定。 如果您將訂單設定設為`Disabled`，商店控制面板上會顯示Amazon訂單，但您必須在[!DNL Amazon Seller Central]帳戶中進行管理。

在Amazon上建立訂單時，不會立即匯入至[!DNL Commerce]。 Amazon會將`Pending`狀態指派給新建立的訂單。 Amazon驗證訂單和付款方法後，訂單的狀態將更改為`Unshipped`。 此狀態更改會觸發訂單導入，而[!DNL Commerce]會建立匹配的相應訂單。

從Amazon匯入的訂單可在[!DNL Commerce] [訂單工作流程](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}中管理。 另請參閱[管理訂單](./managing-orders.md)。

## 配置訂單設定 {#configure-order-settings}

1. 按一下儲存控制面板上的&#x200B;**[!UICONTROL Order Settings]**。

1. 對於&#x200B;**[!UICONTROL Import Amazon Orders]**（必要），選擇一個選項：

   - `Disabled`  — 從Amazon收到新訂單時，選擇您 [!DNL Commerce] 不想在中建立對應訂單的時間。選擇此選項後，此頁上的所有其他欄位都將被禁用。

   - `Enabled`  — （預設）從Amazon收到新訂單時， [!DNL Commerce] 選擇您要建立對應訂單的時間。[!DNL Commerce] 系統會根據Amazon狀態和庫存層級建立訂單。

      >[!NOTE]
      >
      >若要在[!DNL Commerce] [orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}工作流程中管理Amazon訂單，「匯入Amazon訂單」必須設為`Enabled`。 設為`Disabled`時，您的Amazon訂單沒有對應的[!DNL Commerce]訂單編號，且無法在[!DNL Commerce]中管理。 您可以在[!DNL Amazon Seller Central]帳戶中管理這些訂單。

1. 對於&#x200B;**[!UICONTROL Import Amazon Orders Into Magento Store]**，選擇在[!DNL Commerce]中建立對應訂單時，與哪個[!DNL Commerce]儲存Amazon訂單相關聯。

   此設定預設為您在[新增Amazon商店](./store-integration.md)時，所選網站的「商店檢視」。 如果要更改此設定，選項清單取決於您在配置中設定的[!DNL Commerce]儲存。 請參閱[儲存](https://docs.magento.com/user-guide/stores/stores-all-create-view.html#create-a-new-store-view){:target=&quot;_blank&quot;}。

1. 對於&#x200B;**[!UICONTROL Customer Creation]**，選擇一個選項：

   - `No Customer Creation (guest)`  — （預設）選擇您不想在使用Amazon訂單中匯入 [!DNL Commerce] 的客戶資料時建立客戶帳戶。選擇[!DNL Commerce]時，會以與[!DNL Commerce]中處理訪客結帳相同的方式處理匯入的Amazon訂單。

   - `Build New Customer Account`  — 在使用隨Amazon訂單匯入的客戶資料 [!DNL Commerce] 中，選擇您要建立新客戶帳戶的時間。此選項可協助您從Amazon訂單建立客戶資料庫。

1. 對於&#x200B;**[!UICONTROL Order Number Source]**，選擇一個選項：

   - `Build Using Magento Order Number`  — （預設）選擇您何時想使用增量 [!DNL Commerce] 指派的訂單ID，為對應的Amazon訂單建 [!DNL Commerce] 立唯一訂單編號。

   - `Build Using Amazon Order Number`  — 選擇何時使用相 [!DNL Commerce] 應的Amazon分配訂單編號建立訂單編號。
   >[!NOTE]
   >
   >匯入訂單後，Amazon訂單編號會顯示在商店控制面板的&#x200B;_[!UICONTROL Recent Orders]_清單中。 在[!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}工作區中檢視訂單詳細資訊時，會顯示[!DNL Commerce]訂單編號。

1. 對於&#x200B;**[!UICONTROL Order Status]**（必要），選擇一個選項：

   - `Default Order Status`  — （預設）選擇何時要將從Amazon導入的新建立訂單分配給新訂單的定義預設訂單狀態。新訂單的預設狀態（除非您已為新訂單建立自訂訂單狀態）為`Pending`。 請參閱[處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html){:target=&quot;_blank&quot;}。

   - `Custom Order Status`  — 選擇何時要將從Amazon導入的新建立的訂單分配給預設狀態以外的狀態。

   - `Processing Order Status`  — 設為 **[!UICONTROL Order Status]** 時啟 `Custom Order Status`用。選擇您要用於從Amazon匯入的新建立訂單的狀態。 此欄位中的選項基於[!DNL Commerce]中的預設狀態選項。 請參閱[訂單狀態](https://docs.magento.com/user-guide/sales/order-status.html)。 您也可以建立自訂順序狀態，以便在此顯示以供選取。 若要建立自訂訂單狀態，請參閱[自訂訂單狀態](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}。

1. 完成後，按一下&#x200B;**[!UICONTROL Save order settings]**。

![順序設定](assets/amazon-order-settings.png)

| 欄位 | 說明 |
|---|---|
| [!UICONTROL Import Amazon Orders] | 選項：<ul><li>**[!UICONTROL Disabled]**  — 從Amazon收到新訂單時，選擇您 [!DNL Commerce] 不想在中建立對應訂單的時間。選擇此選項後，此頁上的所有其他欄位都將被禁用。</li><li>**[!UICONTROL Enabled]**  — （預設）從Amazon收到新訂單時， [!DNL Commerce] 選擇您要建立對應訂單的時間。[!DNL Commerce] 系統會根據Amazon狀態和庫存層級建立訂單。</li></ul><br><br>`Enabled` 必須選擇以管理中的Amazon訂 [!DNL Commerce]單。選擇`Disabled`時，您的Amazon訂單會顯示在商店控制面板上，但您必須在[!DNL Amazon Seller Central]帳戶中管理訂單。 |
| [!UICONTROL Import Amazon Orders Into Magento Store] | 選擇在[!DNL Commerce] [Orders](https://docs.magento.com/user-guide/sales/orders.html){:target=&quot;_blank&quot;}工作區中建立Amazon訂單時，與哪個[!DNL Commerce]儲存關聯。 此設定預設為當您[新增Amazon商店](./store-integration.md)時，所選[!DNL Commerce]網站的「商店檢視」。 如果要更改此設定，選項清單取決於您在配置中設定的[!DNL Commerce]儲存。 請參閱[儲存](https://docs.magento.com/user-guide/stores/stores-all-stores.html){:target=&quot;_blank&quot;}。 |
| [!UICONTROL Customer Creation] | 選項：<ul><li>**[!UICONTROL No Customer Creation (guest)]**  — （預設）選擇您不想在使用Amazon訂單中匯入 [!DNL Commerce] 的客戶資料時建立客戶帳戶。選取此選項時，此選項會指示[!DNL Commerce]以處理匯入的Amazon訂單，其方式與處理訪客結帳的方式相同。</li><li>**[!UICONTROL Build New Customer Account]**  — 選擇何時要使用隨Amazon訂單匯入的客 [!DNL Commerce] 戶資料在客戶資料庫中建立新客戶帳戶。此選項可協助您從Amazon訂單中建立[!DNL Commerce]客戶資料庫。</li></ul> |
| 訂單編號來源 | 選項：<ul><li>**[!UICONTROL Build Using Magento Order Number]**  — （預設）選擇您何時想使用增量 [!DNL Commerce] 指派的訂單ID，為對應的Amazon訂單建 [!DNL Commerce] 立唯一訂單編號。 </li><li>**使用Amazon訂單編號建置**  — 選擇何時要使用 [!DNL Commerce] 相應的Amazon分配訂單編號建立訂單編號。</li></ul> |
| 待定訂單 | 選項：<ul><li>**[!UICONTROL Do Not Reserve Quantity]**  — 選擇您不希望庫存數量受 [!DNL Commerce] 到Amazon訂單影響的時間。選擇是否將Amazon用於履行流程(FBA)。 選擇並接收Amazon訂單時，訂購數量不會影響[!DNL Commerce]庫存數量。</li><li>**[!UICONTROL Reserve Quantity]**  — 選擇您希望Amazon訂單中的訂單數量在庫存數量中「保留」 [!DNL Commerce] 的時間。當您選擇並收到Amazon訂單時，訂購數量將「保留」您的[!DNL Commerce]庫存數量，以防止您的[!DNL Commerce]庫存「超量銷售」。 「保留」數量無法通過您的[!DNL Commerce]店面購買。</li></ul> |
| [!UICONTROL Order Status] | 選項：<ul><li>**[!UICONTROL Default Order Status]**  — （預設）選擇何時要將從Amazon導入的新建立訂單分配給新訂單的預設訂單狀態。新訂單的預設狀態（除非您已為新訂單建立自訂訂單狀態）為`Pending`。 請參閱[處理訂單](https://docs.magento.com/user-guide/sales/order-processing.html)。</li><li>>**[!UICONTROL Custom Order Status]** — 選擇何時要將從Amazon匯入的新建立訂單指派為預設值以外的狀態。 選擇&#x200B;**[!UICONTROL Processing Order Status]**&#x200B;後，您便可以選擇要用於從Amazon匯入的新建立訂單的狀態。</li></ul> |
| [!UICONTROL Processing Orders Status] | 當&#x200B;_[!UICONTROL Order Status]_設為`Custom Order Status`時啟用。 選擇要分配給新訂單的訂單狀態。 此欄位中的選項取決於[!DNL Commerce]中的預設狀態選項。 請參閱[訂購狀態](https://docs.magento.com/user-guide/sales/order-status.html){:target=&quot;_blank&quot;}。 您也可以建立自訂訂單狀態以顯示在此處。 若要建立自訂訂單狀態，請參閱[自訂訂單狀態](https://docs.magento.com/user-guide/sales/order-status-custom.html){:target=&quot;_blank&quot;}。 |

## [!DNL Commerce] 訂單建立

[!DNL Commerce] 系統會根據下列狀態和庫存條件，為Amazon訂單建立訂單。

### 使用庫存管理建立訂單

>[!NOTE]
>
>僅支援Adobe商務和Magento Open Source2.3.x整合。

| 履行管道 | [!DNL Commerce] 庫存狀態 | Amazon訂單狀態 | [!UICONTROL Create Magento Order] 設定 | 庫存預留 |
|---|---|---|---|---|
| FBA | In-stock<br>Out-of-stock<br>不管理 | 待定 | 否 | 否 |
| FBA | In-stock<br>Out-of-stock<br>不管理 | 待定可用性 | 否 | 否 |
| FBA | In-stock<br>Out-of-stock<br>不管理 | 已取消 | 否 | 否 |
| FBA | In-stock<br>Out-of-stock<br>不管理 | 錯誤 | 否 | 否 |
| FBA | In-stock<br>Out-of-stock<br>不管理 | 未裝運 | 否 | 否 |
| FBA | In-stock<br>Out-of-stock<br>不管理 | 部分已發運 | 否 | 否 |
| FBA | In-stock<br>不管理 | 已發運 | 是 | 否 |
| FBA | 無存貨 | 已發運 | 否 | 否 |
| FBM | In-stock<br>Out-of-stock<br>不管理 | 待定 | 否 | 否 |
| FBM | In-stock<br>Out-of-stock<br>不管理 | 待定可用性 | 否 | 否 |
| FBM | In-stock<br>Out-of-stock<br>不管理 | 已取消 | 否 | 否 |
| FBM | In-stock<br>Out-of-stock<br>不管理 | 錯誤 | 否 | 否 |
| FBM | In-stock<br>不管理 | 未裝運 | 是 | 是 |
| FBM | 無存貨 | 未裝運 | 否 | 否 |
| FBM | In-stock<br>不管理 | 部分已發運 | 是 | 是 |
| FBM | 無存貨 | 部分已發運 | 否 | 否 |
| FBM | In-stock<br>不管理 | 已發運 | 是 | 是 |
| FBM | 無存貨 | 已發運 | 否 | 否 |

>[!NOTE]
>如果以`Partially Shipped`或`Shipped`狀態導入了Amazon訂單，則為訂單中的所有物料建立的庫存保留。 Amazon銷售管道不會補償先前出貨的項目。
>
>如果訂單由Amazon(FBA)履行，但項目處於`out of stock`狀態，則[!DNL Commerce]無法建立對應的訂單。 這是庫存管理整合的限制。
