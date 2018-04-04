---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Preguntas más frecuentes

## ¿Cómo puedo actualizar la información de participación para mis direcciones IP? (SWIP)

El proyecto WhoIs Compartido de ARIN (Shared WhoIs Project - SWIP) le permite proporcionar la información de información de participación para las direcciones IP de su cuenta. Esta herramienta funciona con el Sistema de WHOIS inverso de {{site.data.keyword.BluSoftlayer_notm}}. Se recomienda utilizar ambas herramientas, porque no todas las herramientas de WHOIS utilizan nuestro Sistema de WHOIS inverso para localizar al propietario de un bloque de direcciones IP (una subred). Tenga en cuenta que sólo pueden utilizar el sistema SWIP las subredes con 8 o más direcciones IP (subredes con una máscara de subred más pequeña que 30).

Puede registrar una subred en SWIP yendo a **Red pública -> SWIP** en el Portal del cliente y seleccionando **Subred SWIP** junto al rango de destino.

En la página de SWIP puede realizar las tareas siguientes:

 * **Subred de SWIP:** Enviar una solicitud a ARIN para actualizar su información de direcciones IP con sus datos de WHOIS inverso.<br/>
 * **Actualizar subred:** Actualizar ARIN si sus datos de WHOIS inverso han cambiado.<br/>
 * **Borrar subred:** Eliminar su información de ARIN y sustituirla por la información predeterminada de IBM Cloud.

También puede ver el estado de una solicitud SWIP leyendo la columna de estado en la página de SWIP:

 * **No pasado a Swip:** La solicitud SWIP para esta subred no se ha dado todavía. Los datos de WHOIS mostrarán {{site.data.keyword.BluSoftlayer_notm}} como propietario de la subred.
 * **Solicitud esperando en ARIN...:** Se ha enviado una solicitud, pero estamos esperando una respuesta. Las respuestas pueden tardar hasta tres días.
 * **Borrado esperando en ARIN...:** Al igual que para las solicitudes SWIP, el borrado de la información de WHOIS puede tardar hasta tres días en completarse.
 * **IBM procesando manualmente...:** A veces una solicitud SWIP no puede procesarse automáticamente. En este caso, el error se notifica a {{site.data.keyword.BluSoftlayer_notm}} y tenemos que arreglar la transacción manualmente.
 
