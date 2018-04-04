---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 常見問題

## 如何更新 IP 的所有權資訊？(SWIP)

ARIN 的共用 WhoIs 專案 (SWIP) 可讓您提供帳戶上 IP 位址的所有權資訊。此工具使用 {{site.data.keyword.BluSoftlayer_notm}} Reverse WHOIS 系統。建議使用這兩個工具，因為並非所有 WHOIS 工具都會使用 Reverse WHOIS 系統來尋找 IP（子網路）區塊的擁有者。請注意，只有具有 8 個以上 IP 位址的子網路（子網路遮罩小於 30 的子網路）才能使用 SWIP 系統。

您可以 SWIP 子網路，方法是移至客戶入口網站中的**公用網路 -> SWIP**，然後選取目標範圍旁邊的 **Swip 子網路**。

在 SWIP 頁面上，您可以執行下列作業：

 * **Swip 子網路：**將要求傳送給 ARIN，以使用 Reverse WHOIS 資料來更新 IP 資訊。<br/>
 * **更新子網路：**如果您變更 Reverse WHOIS 資料，請更新 ARIN。<br/>
 * **清除子網路：**從 ARIN 中移除資訊，並將它取代為 IBM Cloud 的預設資訊。

您也可以查看「SWIP 要求」的狀態，方法是讀取 SWIP 頁面上的「狀態」直欄：

 * **未 Swip：**尚未給定此子網路的 SWIP 要求。WHOIS 資料會將 {{site.data.keyword.BluSoftlayer_notm}} 列為子網路的擁有者。
 * **要求 ARIN 上的等待...：**已傳送要求，但我們正在等待回應。回應最多需要三天的時間。
 * **清除 ARIN 上的等待...：**就像 SWIP 要求，清除 WHOIS 資訊最多需要 3 天的時間才能完成。
 * **IBM 手動處理...：**有時，無法自動處理 SWIP 要求。在此情況下，會向 {{site.data.keyword.BluSoftlayer_notm}} 回報錯誤，而且必須手動修正交易。
 
