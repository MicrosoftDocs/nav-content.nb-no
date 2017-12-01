---
title: Serviceordrestatus og reparasjonsstatus
description: Feltet **Status** i vinduet **Serviceordre** og reparasjonsstatusen til servicevaren, som representeres av feltet **Reparasjonsstatuskode** i vinduet **Serviceordre**, har en bestemt forbindelse i Service. Serviceordrestatusen gjenspeiler reparasjonsstatusen til alle servicevarene i serviceordren.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6e2edc1cde66b49c3961cf4c93820f056d230dc8
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="service-order-status-and-repair-status"></a>Serviceordrestatus og reparasjonsstatus
Feltet **Status** i vinduet **Serviceordre** og reparasjonsstatusen til servicevaren, som representeres av feltet **Reparasjonsstatuskode** i vinduet **Serviceordre**, har en bestemt forbindelse i Service. Serviceordrestatusen gjenspeiler reparasjonsstatusen til alle servicevarene i serviceordren.  
  
> [!NOTE]  
>  Disse to statusfeltene har ingen tilknytning til feltet **Frigivelsesstatus** i serviceordrehodet, som styrer hvordan lageret håndterer servicevarer.  
  
 Hver gang reparasjonsstatusen til en servicevare endres i en serviceordre, oppdateres ordrestatusen. Du må angi følgende for å vise statusen som gjenspeiler samlet reparasjonsstatus til hver enkelt servicevare:  
  
* Serviceordrestatusen som hver enkelt reparasjonsstatus er knyttet til. Hvis du vil ha mer informasjon om serviceordrestadier, kan du se Serviceordrestatus.  
* Prioritetsnivået til hvert enkelt alternativ for serviceordrestatus. Hvis du vil ha mer informasjon, kan du se Prioritet.  
  
 Når du konverterer et servicetilbud til en serviceordre, endres reparasjonsstatusen til hver enkelt servicevare i ordren til **Første**, og serviceordren endres til **Ventende**.  
  
## <a name="specifying-service-order-status-for-repair-status"></a>Angi serviceordrestatus for reparasjonsstatus  
Hver enkelt reparasjonsstatus er knyttet til en bestemt serviceordrestatus. Alternativene for serviceordrestatusen er som følger: **I kø**, **I arbeid**, **Avvent** og **Ferdig**. Følgende reparasjonsstatusalternativer finnes: **Første**, **I arbeid**, **Henvist**, **Delvis vedlikeholdt**, **Tilbud ferdig**, **Venter på kunde**, **Reservedel bestilt**, **Reservedel mottatt** og **Ferdig**.  
  
### <a name="pending"></a>I kø  
Serviceordrestatusen **I kø** angir at servicen når som helst kan starte eller fortsette. Alle de fire reparasjonsstatusalternativene **Første**, **Henvist**, **Delvis vedlikehold** og **Reservedel mottatt** kan derfor knyttes til denne serviceordrestatusen.  
  
### <a name="in-process"></a>I arbeid  
Serviceordrestatusen **I arbeid** angir at servicen er i arbeid. Begge de to reparasjonsstatusalternativene **I arbeid** og **Reservedel bestilt** kan derfor knyttes til denne serviceordrestatusen. Hvis du kobler statusen **Reservedel bestilt** til serviceordrestatusen **I arbeid**, må du også koble statusen **Reservedel mottatt** til denne serviceordrestatusen.  
  
### <a name="on-hold"></a>Avvent  
Serviceordrestatusen **Avvent** angir at servicen midlertidig må avventes fordi du venter på et kundesvar eller reservedeler før servicen kan påbegynnes. Alle de tre reparasjonsstatusalternativene **Tilbud ferdig**, **Reservedel bestilt** og **Venter på kunde** kan derfor knyttes til denne serviceordrestatusen.  
  
### <a name="finished"></a>Ferdig  
Serviceordrestatusen **Ferdig** angir at servicen er fullført. Reparasjonsstatusen **Ferdig** er derfor knyttet til denne statusen.  
  
## <a name="assigning-priority-to-service-order-status"></a>Tilordne prioritet til serviceordrestatus  
Når en reparasjonsstatus til en servicevare endres, identifiseres alternativene for serviceordrestatusen som er knyttet til de ulike reparasjonsstatusalternativene for alle servicevarene i ordren. Hvis servicevarene er koblet til to eller flere alternativer for serviceordrestatus, velges serviceordrestatusalternativet med høyest prioritet.  
  
Du må bestemme hvilken serviceordrestatus som inneholder de viktigste opplysningene om statusen til serviceordren, og deretter tilordne denne statusen den høyeste prioriteten og så videre.  
  
### <a name="example"></a>Eksempel  
En vanlig tilordning av prioritetsnivå kan være følgende:  
  
* I arbeid: høy  
* I kø: middels høy  
* Avvent: middels lav  
* Ferdig: lav  
  
Hvis én servicevare for eksempel har reparasjonsstatusen **Første**, knyttet til serviceordrestatusen **I kø**, en annen har reparasjonsstatusen **I arbeid**, knyttet til serviceordrestatusen **I arbeid**, og en tredje har reparasjonsstatusen **Reservedel bestilt**, knyttet til serviceordrestatusen **Avvent**, blir den endelige serviceordrestatusen **I arbeid** fordi denne har høyest prioritet.  
  
## <a name="see-also"></a>Se også  
[Definere statuser for serviceordrer og reparasjoner](service-order-repair-status.md)  
[Konfigurere servicehåndtering](service-setup-service.md)  

