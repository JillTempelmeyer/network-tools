---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Foire aux questions

## Comment mettre à jour les informations de propriété pour mes adresses IP ? (SWIP)

Le projet SWIP (Shared WhoIs Project) d'ARIN vous permet de fournir des informations de propriété pour les adresses IP de votre compte. Cet outil fonctionne avec le système {{site.data.keyword.BluSoftlayer_notm}} Reverse WHOIS. Il est conseillé d'utiliser les deux outils, puisque tous les outils WHOIS ne se servent pas du système Reverse WHOIS pour localiser le propriétaire d'un bloc d'adresses IP (un sous-réseau). Notez que seuls les sous-réseaux avec 8 adresses IP ou plus (sous-réseaux avec un masque de sous-réseau plus petit que 30) peuvent utiliser le système SWIP.

Vous pouvez appliquer un projet SWIP à un sous-réseau en sélectionnant **Réseau public -> SWIP** dans le portail client et en choisissant l'option  **Swip Subnet** en regard de la plage cible.

Sur la page SWIP, vous pouvez effectuer les tâches suivantes :

 * **Swip Subnet :** envoie une demande à ARIN l'invitant à mettre à jour vos informations IP avec vos données Reverse WHOIS.<br/>
 * **Update Subnet :** met à jour ARIN, si vous modifiez vos données Reverse WHOIS.<br/>
 * **Clear Subnet :** retire vos informations depuis ARIN et les remplace avec les informations par défaut d'IBM Cloud.

Vous pouvez également voir l'état d'une demande SWIP en lisant le contenu de la colonne Statut sur la page SWIP :

 * **Not Swipped :** la demande SWIP pour ce sous-réseau n'a pas encore été donnée. Les données répertorieront {{site.data.keyword.BluSoftlayer_notm}} en tant que propriétaire du sous-réseau.
 * **Request waiting on ARIN...: ** une requête a été envoyée mais le système attend une réponse. Les réponses peuvent mettre jusqu'à trois jours à arriver.
 * **Clear waiting on ARIN...: ** comme pour une demande SWIP, la procédure d'effacement des informations WHOIS peut prendre 3 jours à se réaliser.
 * **IBM Manually Processing...: ** il arrive parfois qu'une demande SWIP soit automatiquement traitée. Dans ce cas, l'erreur est signalée à {{site.data.keyword.BluSoftlayer_notm}} et la transaction doit être corrigée manuellement.
 
