---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# FAQ

## 내 IP에 대한 소유권 정보를 어떻게 업데이트할 수 있습니까? (SWIP)

ARIN의 SWIP(Shared WhoIs Project)는 사용자가 자신의 계정의 IP 주소에 대한 소유권 정보를 제공하게 합니다. 이 도구는 {{site.data.keyword.BluSoftlayer_notm}} Reverse WHOIS 시스템과 함께 작동합니다. 모든 WHOIS 시스템이 Reverse WHOIS 시스템을 사용하여 IP 블록(서브넷)의 소유자를 찾지는 않기 때문에 두 도구를 모두 사용할 것을 권장합니다. 8개 이상의 IP 주소를 갖는 서브넷(30개 미만의 서브넷 마스크를 갖는 서브넷)만이 SWIP 시스템을 사용할 수 있음을 주의하십시오. 

고객 포털에서 **공용 네트워크 -> SWIP**로 이동하고 대상 범위 옆에서 **서브넷 Swip**를 선택하여 서브넷을 SWIP할 수 있습니다. 

SWIP 페이지에서 다음 태스크를 수행할 수 있습니다. 

 * **서브넷 Swip:** Reverse WHOIS 데이터로 IP 정보를 업데이트하는 요청을 ARIN으로 보냅니다. <br/>
 * **서브넷 업데이트:** Reverse WHOIS 데이터를 변경하는 경우 ARIN을 업데이트합니다. <br/>
 * **서브넷 지우기:** ARIN에서 사용자의 정보를 제거하고 IBM Cloud의 기본 정보로 대체합니다. 

또한 SWIP 페이지의 상태 열을 읽고 SWIP 요청의 상태를 볼 수도 있습니다. 

 * **Swip되지 않음:** 이 서브넷의 SWIP 요청이 아직 제공되지 않았습니다. WHOIS 데이터는 {{site.data.keyword.BluSoftlayer_notm}}를 서브넷의 소유자로 나열합니다. 
 * **ARIN에서 요청 대기 중...:** 요청이 전송되었지만, 응답을 대기 중입니다. 응답은 최대 3일이 걸릴 수 있습니다. 
 * **ARIN에서 지우기 대기 중...:** SWIP 요청과 같이 WHOIS 정보 지우기도 완료하는 데에 최대 3일이 걸릴 수 있습니다. 
 * **IBM 수동 처리 중...:** 때로는 SWIP 요청이 자동으로 처리될 수 없습니다. 이 경우 오류가 {{site.data.keyword.BluSoftlayer_notm}}에 보고되며 수동으로 트랜잭션을 수정해야 합니다. 
 
