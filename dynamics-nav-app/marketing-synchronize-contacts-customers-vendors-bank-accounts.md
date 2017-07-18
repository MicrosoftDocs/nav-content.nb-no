---
title: "Synkronisere kontakter med kunder, leverandører og bankkonti"
author: edupont04
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ea22e27e3dd5a5698a37113cb1df3e408e544ddd
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---
# <a name="synchronizing-contacts-with-customers-vendors-and-bank-accounts"></a>Synkronisere kontakter med kunder, leverandører og bankkonti
Hvis en del av kontaktene også er kunder, leverandører eller bankkonti, kan du synkronisere kontaktinformasjonen med relatert kunde, leverandør eller bankkonto. Synkronisering gjør at informasjon som er felles mellom kontakter og kunder, leverandører eller bankkonto, er den samme.  

Før du kan synkronisere kontaktene med kunder, leverandører eller bankkonti, må du angi en kode for forretningsforbindelse for kunder, leverandører og bankkonti i vinduet **Markedsføringsoppsett**. Hvis du vil ha mer informasjon, kan du se [Konfigurere markedsføring og kontaktbehandling](marketing-setup-marketing.md).

## <a name="different-ways-to-synchronize-contacts-with-customers-vendors-and-bank-accounts"></a>Ulike metoder for å synkronisere kontakter med kunder, leverandører og bankkonti
Du kan synkronisere kontaktene med kunder, leverandører eller bankkonti ved hjelp av tre metoder:

* Koble kontakter til eksisterende kunder, leverandører og/eller bankkonti fra kontaktkortet. Hvis du vil ha mer informasjon, kan du se [Knytte kontakter til kunder, leverandører og bankkonti](marketing-how-link-contact.md).
* Opprett kunder, leverandører eller bankkonti fra kontakten. Hvis du vil ha mer informasjon, kan du se [Opprette en kunde, leverandør eller bankkonto fra en kontakt](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).
*  Opprett kontakter fra kunder, leverandører eller bankkonti. Hvis du vil ha mer informasjon, kan du se [Opprette en selskapskontakt fra kunde, leverandør eller bankkonto](marketing-how-create-contact-companies.md).

## <a name="consequences-of-synchronization"></a>Konsekvensene av synkronisering
Når kontakten synkroniseres med kunde, leverandør, bankkonto:

* Du trenger du bare å oppdatere opplysninger på ett sted. Hvis du for eksempel endrer telefonnummeret på kontakten, blir telefonnummeret automatisk oppdatert med de samme endringene på kunden, leverandøren eller bankkontoen.
* Hvis du har angitt en nummerserie for kontakter, opprettes det automatisk et kontaktkort for kunden, leverandøren eller bankkontoen når du oppretter et kundekort, leverandørkort eller bankkontokort.
* Du kan du opprette tilbud og ordrer og forespørsler og bestillinger fra kontakten.
*  Du kan angi at samhandlinger registreres når du utfører handlinger, for eksempel når du skriver ut ordrer, rammeordrer, oppretter serviceordrer, sender e-post og så videre.
* Hvis du sletter en kontakt som er koblet til en kunde, leverandør eller bankkonto, er det bare kontakten som fjernes. Kunden, leverandøren eller bankkontoen beholdes.
* Hvis du sletter en kunde, leverandør eller bankkonto som er koblet til en kontakt, beholdes kontakten.

**Merk**: Noen detaljer, for eksempel fakturerings- og bokføringsopplysninger, vises ikke på kontaktkortet. Du vil derfor kanskje legge dem til manuelt på kundekortet, leverandørkortet eller bankkontokortet når du oppretter kontakter som kunder, leverandører eller bankkonti.

##<a name="see-also"></a>Se også
[Administrere kontakter](marketing-contacts.md)

