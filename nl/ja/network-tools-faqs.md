---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# FAQ

## 自分の IP の所有権情報を更新するには、どうすればよいですか? (SWIP)

ARIN の Shared WhoIs Project (SWIP) を使用すると、アカウントの IP アドレスの所有権情報を提供できます。このツールは、{{site.data.keyword.BluSoftlayer_notm}} Reverse WHOIS システムで動作します。IP のブロック (サブネット) の所有者を見つけるためにすべての WHOIS ツールが Reverse WHOIS システムを使用するとは限らないため、両方のツールを使用することをお勧めします。8 個以上の IP アドレスを持つサブネット (サブネット・マスクが 30 より小さいサブネット) のみが SWIP システムを使用できることに注意してください。

カスタマー・ポータルで**「パブリック・ネットワーク (Public Network)」 -> 「SWIP」**に移動し、ターゲット範囲の横にある**「サブネットに対して SWIP を実行 (Swip Subnet)」**を選択すると、サブネットに対して SWIP を実行できます。

「SWIP」ページでは、以下のタスクを実行できます。

 * **サブネットに対して SWIP を実行 (Swip Subnet):** Reverse WHOIS データを使用して IP 情報を更新する要求を ARIN に送信します。<br/>
 * **サブネットの更新 (Update Subnet):** Reverse WHOIS データを変更した場合は、ARIN を更新します。<br/>
 * **サブネットのクリア (Clear Subnet):** ARIN から情報を削除し、IBM Cloud のデフォルト情報に置き換えます。

「SWIP」ページの状況列を読み取ることによって、SWIP 要求の状態を確認することもできます。

 * **SWIP 未実行 (Not Swipped):** このサブネットに対する SWIP 要求はまだ実行されていません。WHOIS データは、サブネットの所有者として {{site.data.keyword.BluSoftlayer_notm}} をリストします。
 * **ARIN で要求を待機中... (Request waiting on ARIN...):** 要求は送信されましたが、応答待ちです。応答までに最長 3 日かかることがあります。
 * **ARIN でクリアを待機中... (Clear waiting on ARIN...):** ちょうど SWIP 要求と同じように、WHOIS 情報のクリアには、完了まで最長 3 日かかることがあります。
 * **IBM が手動で処理中... (IBM Manually Processing...):** 時には SWIP 要求が自動的に処理されないことがあります。この場合、{{site.data.keyword.BluSoftlayer_notm}} にエラーが報告され、トランザクションを IBM で手動で修正する必要があります。
 
