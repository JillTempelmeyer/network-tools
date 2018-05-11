---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Domande frequenti

## Come posso aggiornare le informazioni di proprietà per i miei IP? (SWIP)

SWIP (Shared WhoIs Project) di ARIN ti consente di fornire informazioni di proprietà per gli indirizzi IP nel tuo account. Questo strumento funziona con il sistema Reverse WHOIS (WHOIS inverso) di {{site.data.keyword.BluSoftlayer_notm}}. Si consiglia di utilizzare entrambi gli strumenti perché non tutti gli strumenti WHOIS utilizzano il nostro sistema Reverse WHOIS per individuare il proprietario di un blocco di IP (una sottorete). Nota: solo le sottoreti con 8 indirizzi IP o più (sottoreti con una maschera di sottorete inferiore a 30) possono utilizzare il sistema SWIP.

Puoi eseguire lo SWIP di una sottorete andando a **Public Network -> SWIP** nel Portale del cliente e selezionando **Swip Subnet** accanto all'intervallo di destinazione.

Nella pagina SWIP puoi eseguire queste attività:

 * **Swip Subnet:** Invia una richiesta ad ARIN per aggiornare le tue informazioni IP con i tuoi dati Reverse WHOIS.<br/>
 * **Update Subnet:** Aggiorna ARIN, se modifichi i tuoi dati Reverse WHOIS (WHOIS inverso).<br/>
 * **Clear Subnet:** Rimuovi le tue informazioni da ARIN e sostituiscile con le informazioni predefinite di IBM Cloud.

Puoi anche vedere lo stato di una richiesta SWIP leggendo la colonna Status nella pagina SWIP:

 * **Not Swipped:** La richiesta SWIP per questa sottorete non è stata ancora fornita. I dati WHOIS elencheranno {{site.data.keyword.BluSoftlayer_notm}} come proprietario della sottorete.
 * **Request waiting on ARIN...:** È stata inviata una richiesta ma stiamo aspettando una risposta. Le risposte possono richiedere fino a tre giorni.
 * **Clear waiting on ARIN...:** Proprio come nel caso di una richiesta SWIP, il completamento della cancellazione delle informazioni WHOIS può richiedere fino a tre giorni.
 * **IBM Manually Processing...:** A volte non è possibile elaborare automaticamente una richiesta SWIP. In questo caso, l'errore viene segnalato a {{site.data.keyword.BluSoftlayer_notm}} e dobbiamo correggere manualmente la transazione.
 
