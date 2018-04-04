---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 常见问题

## 如何更新我的 IP 所有权信息？(SWIP)

ARIN 的共享 WhoIs 项目 (SWIP) 允许您提供帐户 IP 地址的所有权信息。此工具与 {{site.data.keyword.BluSoftlayer_notm}} Reverse WHOIS 系统一起使用。建议同时使用这两种工具，因为并非所有 WHOIS 工具都使用 Reverse WHOIS 系统来查找 IP 块（子网）的所有者。请注意，只有具有 8 个或更多 IP 地址的子网（子网掩码小于 30 的子网）才能使用 SWIP 系统。

您可以在客户门户网站中，转至**公用网络 -> SWIP**，并选择目标范围旁边的 **Swip 子网**来对子网执行 SWIP。

在 SWIP 页面上，可执行以下任务：

 * **Swip 子网：**向 ARIN 发送请求，以使用 Reverse WHOIS 数据来更新 IP 信息。<br/>
 * **更新子网：**更新 ARIN（如果更改了 Reverse WHOIS 数据）。<br/>
 * **清除子网：**从 ARIN 中除去您的信息，并替换为 IBM Cloud 的缺省信息。

您还可以通过查看 SWIP 页面上的“状态”列来了解 SWIP 请求的状态：

 * **未执行 SWIP：**尚未发出对此子网的 SWIP 请求。WHOIS 数据会将 {{site.data.keyword.BluSoftlayer_notm}} 列为子网的所有者。
 * **请求正在等待 ARIN...：**请求已发送，但正在等待响应。响应最长可能需要 3 天时间。
 * **清除操作正在等待 ARIN...：**与 SWIP 请求一样，清除 WHOIS 信息最长可能需要 3 天才能完成。
 * **IBM 手动处理中...：**有时 SWIP 请求无法自动处理。在这种情况下，会向 {{site.data.keyword.BluSoftlayer_notm}} 报告错误，并且我们必须手动修复该事务。
 
