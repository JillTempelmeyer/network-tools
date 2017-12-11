---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# FAQs

## How can I update the ownership information for my IPs? (SWIP)

ARIN's Shared WhoIs Project (SWIP) lets you provide ownership information for IP addresses on your account. This tool works with the {{site.data.keyword.BluSoftlayer_notm}} Reverse WHOIS system. It is recommended to use both tools, because not all WHOIS tools use our Reverse WHOIS system to locate the owner of a block of IPs (a subnet). Note that only subnets with 8 IP addresses or more (subnets with a subnet mask smaller than 30) can use the SWIP system.

You may SWIP a subnet by going to **Public Network -> SWIP** in the customer portal and selecting **Swip Subnet** next to the target range.

On the SWIP page you may perform the following tasks:

 * **Swip Subnet:** Send a request to ARIN to update your IP information with your Reverse WHOIS data.<br/>
 * **Update Subnet:** Update ARIN, if you change your Reverse WHOIS data.<br/>
 * **Clear Subnet:** Remove your information from ARIN and replace it with IBM Cloud's default information.

You can also see the state of a SWIP Request by reading the Status column on the SWIP page:

 * **Not Swipped:** The SWIP request for this subnet has not been given yet. WHOIS data will list {{site.data.keyword.BluSoftlayer_notm}} as the owner of the subnet.
 * **Request waiting on ARIN...:** A request has been sent, but we're waiting for a response. Responses can take up to three days.
 * **Clear waiting on ARIN...:** Just like a SWIP request, clearing out the WHOIS information can take up to 3 days to complete.
 * **IBM Manually Processing...:** Sometimes a SWIP request can't be automatically processed. In this case, the error is reported to {{site.data.keyword.BluSoftlayer_notm}} and we must manually fix the transaction.
 
