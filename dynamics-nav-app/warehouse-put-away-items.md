---
title: Plassere varer
description: "Lageraktiviteten med å plassere varer etter at de er mottatt eller uttatt, utføres på ulike måter avhengig av hvordan lagerstyringsfunksjonene er satt opp."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0b68ef1b4c73eef1ac82d59587011a0fcdead096
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="putting-items-away"></a>Plassere varer
Lageraktiviteten med å plassere varer etter at de er mottatt eller uttatt, utføres på ulike måter avhengig av hvordan lagerstyringsfunksjonene er satt opp. Kompleksiteten kan variere fra ingen lagerfunksjoner, via grunnleggende lagerkonfigurasjoner der bestilling for bestilling behandles ved hjelp av bare en eller flere aktiviteter, til avanserte oppsett der alle lageraktiviteter utføres i en styrt arbeidsflyt. Du finner mer informasjon under [Definere lagerstyring](warehouse-setup-warehouse.md).

Hvis du velger å organisere og registrere plasseringsopplysninger med lagerdokumenter, setter du en hake i feltet **Plassering nødv.** på lokasjonskortet. Det betyr at når varer kommer inn på lagerlokasjonen via et inngående kildedokument, vil du at plukkingen av disse varene skal kontrolleres av systemet. Et inngående kildedokument kan være en bestilling, en ordreretur, en inngående overføringsordre eller en produksjonsordre med avgang som er klar til plassering.  

Hvis lokasjonen er definert til å bruke plasseringsbehandling, men ikke mottaksbehandling, bruker du vinduet **Lagerplassering** til å organisere opplysningene om plasseringen, skrive dem ut, angi resultatet av den aktuelle plasseringen og bokføre plasseringsopplysningene, noe som fører til at mottaksopplysningene for kildedokumentet bokføres. Når det gjelder en produksjonsordre, bokfører bokføringsprosessen avgangen for ordren og fullfører produksjonsordren.

Hvis lokasjonen er definert til å kreve både mottaksbehandling og plasseringsbehandling, det vil si at du har merket av for feltet **Mottak nødv.** og **Plassering nødv.** på lokasjonskortet, bruker du en annen fremgangsmåte når du plasserer varer. I dette tilfellet vil du bruke **Plassering**-vinduet til å håndtere plasseringen. Plassering fungerer på samme måte som Lagerplassering, bortsett fra at du registrerer plasseringen i stedet for å bokføre opplysninger om den. Merk at registrering av lagerplassering ikke bokfører mottaket av varene. Den bare oppdaterer hylleinnholdet. Som lagerleder kan du bruke plasseringsforslag til å organisere opplysninger om plassering før du oppretter de enkelte plasseringsinstruksjonene.

Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.   

|**Hvis du vil**|**Se**|  
|------------|-------------|  
|Bokfør mottaket av varer direkte fra det inngående bestillingsdokumentet og dermed registrer plasseringen, fordi det ikke finnes noe lageroppsett.|[Motta varer](warehouse-how-receive-items.md)|  
|Plassere varer bestilling for bestilling, og bokføre mottaket i samme aktivitet, i et grunnleggende lageroppsett.|[Plassere varer med lagerplasseringer](warehouse-how-to-put-items-away-with-inventory-put-aways.md)|  
|Plassere varer for flere ordrer i et avansert lageroppsett.|[Plassere varer med lagerplasseringer](warehouse-how-to-put-items-away-with-warehouse-put-aways.md)|  
|Plasser produserte eller monterte varer i et enkelt eller avansert lageroppsett.|[Plassere produksjonsavgang eller monteringsavgang](warehouse-how-to-put-away-production-output.md)|
|Planlegge optimaliserte plasseringsinstruksjoner for flere bokførte lagermottak, i stedet for at lagermedarbeiderne skal gjøre dette ved mottak.|[Planlegge plasseringer i forslag](warehouse-how-to-plan-put-aways-in-worksheets.md)|  
|Sette tilbake varer som ble plukket automatisk ved hjelp av en intern plukk, for eksempel til en produksjonsordre som ikke forbrukte det forventede antallet.|[Plukke og plassere uten et kildedokument.](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|Dele en plasseringslinje for å plassere en del av antallet i plasseringen i tilgjengelige hyller, fordi den angitte hyllen er full.|[Dele lageraktivitetslinjer](warehouse-how-to-split-warehouse-activity-lines.md)|
|Få tilgang umiddelbart til plasseringer som er tilordnet til deg som lagermedarbeider.|[Finne lageroppgavene dine](warehouse-how-to-find-your-warehouse-assignments.md)|    

## <a name="see-also"></a>Se også  
[Lagerstyring](warehouse-manage-warehouse.md)  
[Lager](inventory-manage-inventory.md)  
[Definere lagerstyring](warehouse-setup-warehouse.md)     
[Monteringsstyring](assembly-assemble-items.md)    
[Designdetaljer: Lagerstyring](design-details-warehouse-management.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

