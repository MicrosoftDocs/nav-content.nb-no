---
title: Administrere kunder ved hjelp av Dynamics 365 for Sales
description: "Du kan bruke Dynamics 365 for Sales fra Dynamics NAV for å tilordne data og få sømløs integrasjon og synkronisering i interessent-til-kontanter-prosessen."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: integration, synchronize, map
ms.date: 06/06/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f3c9cff4094395a1f06ba04ba2476de76c4a04a1
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="managing-your-customer-relationships-using-dynamics-365-for-sales-from-inside-dynamics-nav"></a>Administrere kunderelasjoner ved hjelp av Dynamics 365 for Sales fra Dynamics NAV
Hvis du bruker Dynamics 365 for Sales til kundeengasjement, kan du bruke [!INCLUDE[d365fin](includes/d365fin_md.md)] for ordrebehandling og økonomi og få sømløs integrasjon i kundeemne-til-kontanter-prosessen.

Når programmet er konfigurert til å integrere med Dynamics 365 for Sales, har du tilgang til salgstall fra [!INCLUDE[d365fin](includes/d365fin_md.md)] og motsatt vei i noen tilfeller. Denne integrasjonen gjør at du kan arbeide med og synkronisere datatyper som er felles for begge tjenester, for eksempel kunder, kontakter og salgsinformasjon, og hold dataene oppdaterte på begge lokasjoner.  

Selgeren i Dynamics 365 for Sales kan for eksempel bruke prislister fra [!INCLUDE[d365fin](includes/d365fin_md.md)] når de oppretter en salgsordre. Når de legger til varen på salgsordrelinjen i Dynamics 365 for Sales, kan de også se lagernivået (tilgjengelighet) av varen fra [!INCLUDE[d365fin](includes/d365fin_md.md)]. Disse dataene er publisert som en del av den assisterte installasjonsveiledningen **Tilkoblingsoppsett for Dynamics 365**.  

## <a name="setting-up-the-connection"></a>Definere tilkoblingen
Fra startsiden kan du få tilgang til **Tilkoblingsoppsett for Dynamics 365** assistert oppsettguide som hjelper deg med å konfigurere tilkoblingen. Når dette er gjort, vil du ha en sømløs kobling i Dynamics 365 for Sales-oppføringer med [!INCLUDE[d365fin](includes/d365fin_md.md)]-poster.  

> [!NOTE]  
>   Det følgende forklarer det assisterte oppsettet, men du kan utføre de samme oppgavene manuelt i vinduet **Konfigurasjon for Dynamics 365-tilkobling**.

Du kan velge hvilke data som skal synkroniseres mellom de to tjenestene i den assisterte oppsettguiden. Du kan også angi at du vil importere din eksisterende Dynamics 365 for Sales-løsning. I så fall må du angi en administrativ brukerkonto.

### <a name="setting-up-the-user-account-for-importing-the-solution"></a>Konfigurere kontoen for import av løsning
Hvis du vil importere en eksisterende Dynamics 365 for Sales-løsning, bruker oppsettguiden en administrativ konto. Denne kontoen må være en gyldig bruker i Dynamics 365 for Sales med følgende sikkerhetsroller:

* Systemansvarlig  
* Løsningstilpasser  

Hvis du vil ha mer informasjon, kan du se [Opprette brukere og tilordne sikkerhetsroller for Microsoft Dynamics NAV (online) ](https://technet.microsoft.com/library/jj191623.aspx)på techNet og [Administrere brukere og tillatelser](ui-how-users-permissions.md).  

Denne kontoen brukes bare under oppsettet. Når løsningen er importert til [!INCLUDE[d365fin](includes/d365fin_md.md)], er kontoen ikke lenger nødvendig.

### <a name="setting-up-the-user-account-for-synchronization"></a>Konfigurere kontoen for synkronisering
Integreringen er avhengig av en delt brukerkonto. Så i Office 365-abonnementet, må du opprette et engasjert personell som skal brukes for synkronisering mellom de to tjenestene. Denne kontoen må være en gyldig bruker i Dynamics 365 for Sales allerede, men du trenger ikke å tilordne sikkerhetsroller til kontoen fordi installasjonsprogrammet for TV-guiden gjør dette for deg. Du må angi denne kontoen én eller flere ganger i installasjonsveiledningen, avhengig av hvor mye synkroniseringen du vil aktivere. Hvis du vil ha mer informasjon, kan du se [Opprette brukere og tilordne sikkerhetsroller for Microsoft Dynamics NAV (online) ](https://technet.microsoft.com/library/jj191623.aspx) på techNet.

Hvis du velger å aktivere *Varedisposisjon*, må integrasjonsbrukerkontoen ha en tilgangstast for webtjenester. Dette er en totrinns ting på siden [!INCLUDE[d365fin](includes/d365fin_md.md)] for denne brukerkontoen, må du velge knappen **Endre webtjenestenøkkel**, og i oppsettguiden for tilkobling av Dynamics 365 må du angi brukeren som OData-webtjenestebrukeren.

Hvis du velger å aktivere *ordrerintegrering*, må du angi en bruker som kan håndtere denne synkroniseringen - integreringsbrukeren eller en annen brukerkonto.

### <a name="coupling-records"></a>Koblingsposter
Du kan velge å synkronisere mellom de to tjenestene i den assisterte oppsettguiden. Men senere kan du også definere synkronisering av bestemte typer data. Dette kalles *kobling*, og denne delen inneholder anbefalinger om hva du må ta i betraktning.

Hvis du vil vise Dynamics 365 for Sales-kontoer som kunder i for eksempel [!INCLUDE[d365fin](includes/d365fin_md.md)], må du koble to typer poster. Det er ikke veldig komplisert - du åpner **Kundeoversikt**-vinduet i [!INCLUDE[d365fin](includes/d365fin_md.md)], og det er en handling i båndet for å koble disse dataene med Dynamics 365 for Sales. Deretter angir du hvilke [!INCLUDE[d365fin](includes/d365fin_md.md)]-kunder som samsvarer med hvilke konti i Dynamics 365 for Sales.

I enkelte områder avhenger funksjonaliteten av at du kobler noen bestemte sett med data før andre sett med data, som vist i følgende liste:

* Kunder og konti  
  * Koble selgere med Dynamics 365 for Sales-brukere først  
* Varer og ressurser  
  * Koble målenheter med Dynamics 365 for Sales-enhetsgrupper først  
* Varer og ressurspriser  
  * Koble kundeprisgrupper med Dynamics 365 for Sales-priser først  

> [!NOTE]  
>   Hvis du bruker priser i fremmed valuta, må du kontrollere at du kobler valutaer til Dynamics 365 for Sales-transaksjonsvalutaer.

Dynamics 365 for Sales-salgsordrer avhenger av ekstra informasjon, for eksempel kunder, målenheter, valutaer, kundeprisgrupper, varer og/eller ressurser. For at Dynamics 365 for Sales-salgsordrer skal fungere sømløst sammen, må du koble kunder, målenheter, valutaer, kundeprisgrupper, varer og/eller ressurser først.

### <a name="synchronizing-records-fully"></a>Fullstendig synkronisering av oppføringer
Til slutten av den assisterte oppsettguiden, kan du velge **Kjør full synkronisering** for å starte synkronisering av alle [!INCLUDE[d365fin](includes/d365fin_md.md)]-poster med alle relaterte poster i den tilkoblede Dynamics 365 for Sales-løsningen. I vinduet **Gjennomgang av full synkronisering for CRM** velger du **Start**-handlingen. Deretter synkroniseringen begynner å utføre jobber i henhold til avhengighetene. Hvis du for eksempel synkroniseres valuta poster før kundeoppføringer. Fullstendig synkronisering kan ta lang tid, og derfor kjører i bakgrunnen, slik at du kan fortsette å arbeide [!INCLUDE[d365fin](includes/d365fin_md.md)].

Hvis du vil kontrollere fremdriften for individuelle prosjekter i en fullstendig synkronisering, detaljer for den **Status for jobben køen**, **til Int. tabellen Jobbstatus**, eller **fra Int. tabellen Jobbstatus** i den **CRM Full synkronisering. Se gjennom** vindu.

Fra vinduet **Tilkoblingsoppsett for Dynamics 365** kan du få detaljer om fullstendig synkronisering når som helst. Herfra kan du også åpne **Tilordninger for integreringstabell**-vinduet for å se detaljer om tabellene i Dynamics NAV og i Dynamics 365 for Sales-løsningen som må synkroniseres.

## <a name="see-also"></a>Se også
[Forbindelser](marketing-relationship-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)  
[Administrere brukere og tillatelser](ui-how-users-permissions.md)    
[Introduser organisasjonen og brukerne for Dynamics NAV (online)](https://www.microsoft.com/en-US/Dynamics/crm-customer-center/onboard-your-organization-and-users-to-dynamics-365-online.aspx)  

##

