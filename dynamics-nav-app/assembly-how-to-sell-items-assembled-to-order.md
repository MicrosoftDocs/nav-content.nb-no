---
title: Selge varer som er montert til ordre
description: "Hvis varen er definert for Monter til ordre, forventes varen ikke å være på lager, og den må monteres spesifikt for en ordre. Når du angir varen på en ordrelinje, blir en monteringsordre automatisk opprettet og koblet til ordren."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fc140a0fa7d58c38234f67471323241ac94ca489
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-sell-items-assembled-to-order"></a>Selge varer som er montert til ordre
Hvis **Monteringsprinsipp**-feltet på varekortet for en monteringsvare er **Monter til ordre**, forventes varen ikke å være på lager, og den må monteres spesifikt for en ordre. Når du angir varen på en ordrelinje, blir en monteringsordre automatisk opprettet og koblet til ordren.  

> [!NOTE]  
>  Hvis noen montere-til-ordre-varer allerede er på lager, kan du trekke dette antallet fra monteringsordren og reservere det fra beholdningen. Hvis du vil ha mer informasjon, kan du se [Selge lagervarer i montere-til-ordre-flyter](assembly-how-to-sell-assemble-to-order-items-and-inventory-items-together.md).  

I denne fremgangsmåten behandler du salget av en vare som skal monteres i henhold til spesifikasjonene kunden har bedt om. Trinnene inkluderer start av ordrelinjen, tilpasning av monteringsvaren ved å redigere tilhørende komponenter og ressurser, kontroll av tilgjengeligheten for å fastsette en leveringsdato og frigivelse av ordren for montering og umiddelbar levering.  

> [!NOTE]  
>  Følgende fremgangsmåte omfatter ikke standardtrinnene for ordrer før trinnet der du angir montere-til-ordre-varen på en ordrelinje.  

## <a name="to-sell-an-item-that-is-assembled-to-order"></a>Selge en vare som er montert til ordre  
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Ordrer**, og velg deretter den relaterte koblingen.  
2.  Opprett en ordre. Hvis du vil ha mer informasjon, kan du se [Selge produkter](sales-how-sell-products.md).  
3.  I feltet **Nr.** -feltet angir du en vare som er definert for å monteres til ordre.  
4.  Definer hvilken lokasjon varen skal selges fra, i **Lokasjonskode**-feltet. Monteringsprosessen vil skje på den lokasjonen.  
5.  Angi hvor mange enheter som skal selges, i **Antall**-feltet.  

    > [!NOTE]  
    >  Hvis én eller flere komponenter i det forespurte monteringsvareantallet ikke er tilgjengelige, åpnes et vindu med en tilgjengelighetsadvarsel. Hvis du vil ha mer informasjon, se Montering – tilgjengelighet.  

    En montersordre opprettes nå automatisk og kobles til ordrelinjen. Forfallsdatoen for denne monteringsordren synkroniseres med forsendelsesdatoen på ordrelinjen.  

    Antallet som skal selges, kopieres til feltet **Ant. å montere til ordre**, som angir at vareoppsettet forventer at hele antallet på salgslinjen skal monteres til ordren. Du kan redusere antallet for montere til ordre, for eksempel hvis du vet at enkelte varer allerede er tilgjengelige. Hvis du vil ha mer informasjon, kan du se [Selge lagervarer i montere-til-ordre-flyter](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).  

6.  For å gjenspeile at kunden ønsker en ekstra vare i et sett, går du til hurtigfanen **Linjer**, velger **Linje**, velger **Monter til ordre** og velger deretter **Montere til ordre-linjer** for å vise og endre standard monteringskomponenter. Du kan også merke feltet **Ant. som skal monteres til ordre**.  
7.  Opprett en ny linje av typen **Vare** for det forespurte tilleggsinnholdet i settet i vinduet **Montere til ordre – linjer**. Linjen representerer en ekstra monteringskomponent.  

    Du kan også tilpasse rekkefølgen ved å øke antallet for én standardvare i settet. Du kan gjøre dette ved å øke verdien i **Antall per**-feltet på den bestemte monteringsordrelinjen.  

    > [!NOTE]  
    >  Vinduet **Monteringsordrelinjene** inneholder de grunnleggende feltene som en selger forventes å bruke for å tilpasse komponentlisten, legge til varesporingsnumre eller løse problemer med komponenttilgjengelighet. Hvis du vil vise mer informasjon om monteringsordren, for eksempel startdatoen for den, velger du **Vis dokumenter** under **Prosess** i kategorien **Hjem**. Dette åpner en full visning av monteringsordren som er knyttet til ordrelinjen. Du kan ikke endre innholdet i de fleste av feltene i monteringsordrehodet, og du kan ikke bokføre monteringsavgang herfra fordi du må bruke leveringsbokføring for ordrelinjen.  
    >   
    >  I hodet til koblede monteringsordrer der det bare **Startdato**-feltet som kan endres for at monteringsarbeidere kan angi en tidligere dato enn forfallsdatoen når de vil starte prosessen. Alle feltene på linjene i den tilknyttede monteringsordren kan endres slik at lagermedarbeidere kan angi forbruksverdier under prosessen.  

8.  Se gjennom eller reager på problemer med komponententilgjengelighet Velg for eksempel en disponibel erstatningsvare, eller opprett en senere forfallsdato.  
9. Lukk vinduet **Montere til ordre – linjer**. Den koblede monteringsordren er nå klar til å begynne å montere de tilpassede elementene etter forfallsdatoen.  
10. På ordren velger du **Frigi** for å varsle monteringsavdelingen om at monteringsprosessen kan starte.  
11. Utfør trinnene for montering av varer som selges i denne fremgangsmåten, i monteringsavdelingen. Hvis du vil ha mer informasjon, kan du se [Montere varer](assembly-how-to-assemble-items.md).  

## <a name="see-also"></a>Se også  
[Monteringsstyring](assembly-assemble-items.md)  
[Arbeide med stykklister](inventory-how-work-BOMs.md)  
[Lager](inventory-manage-inventory.md)  
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

