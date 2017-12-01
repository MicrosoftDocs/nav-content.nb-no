---
title: "VIA-metoder for å beregne og registrere prosjektfremdrift"
description: "Beskriver de forskjellige VIA-metodene (varer i arbeid) du kan bruke til å bokføre, overvåke og beregne økonomiske opplysninger for prosjekter som pågår."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: work in process, work in progress, calculate project WIP
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 4a472d7a45cacfe4cd2534747f447a1e4ca7a303
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-wip-methods"></a>Forstå VIA-metoder
[!INCLUDE[d365fin](includes/d365fin_md.md)] støtter følgende måter å beregne og registrere verdien av varer i arbeid på.

| VIA-metode | Beregningsformel | Beskrivelse av beregning |
| --- | --- | --- |
| Kostverdi |Ført inntekt = fakturerbar fakturert pris<br /><br /> Anslått kostbeløp = fakturerbart (salgsbeløp) x budsjett (kostforhold)<br /><br /> VIA-kost = (løpende – fakturert %) x anslått kostbeløp<br /><br /> Løpende = forbruk (kostbeløp) / budsjett (kostbeløp)<br /> Fakturert % = fakturerbar (fakturert pris)<br /><br /> Fakturerbar (salgsbeløp) ført kost = forbruk totale kostnader - VIA |Kostverdiberegninger starter med å beregne verdien av det som er oppgitt, ved å ta en andel av anslått kostbeløp basert på prosent fullført. Fakturert kost trekkes fra ved å ta en andel av anslått kostbeløp basert på fakturert prosent.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet, budsjettsalgsbeløpet og budsjettkostbeløpet angis riktig for hele prosjektet. |
| Kostnad for salg |Ført inntekt = fakturerbar fakturert pris<br /><br /> Ført kost = budsjett (kostbeløp) x fakturert prosent<br /><br /> Fakturert % = fakturerbar (fakturert pris) / fakturerbar (salgsbeløp)<br /><br /> (Fakturert % finnes som en kolonne på prosjektoppgavelinjer)<br /><br /> VIA-kost = forbruk (kostbeløp) - ført kost |Beregning av solgte varers innkjøps- eller produksjonspris begynner ved å beregne ført kost. Kost føres proporsjonalt basert på budsjettkostbeløp.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet og budsjettkostbeløpet angis riktig for hele prosjektet. |
| Salgsverdi |Ført kost = forbruk (kostbeløp)<br /><br /> Ført inntekt = forbruk (salgsbeløp) x forventet faktureringsforhold<br /><br /> Kostgjenopprettingsprosent = fakturerbar (salgsbeløp) / budsjett (salgsbeløp)<br /><br /> VIA-salg = ført salg - fakturerbar (fakturert pris) |Salgsverdiberegninger fører inntekt proporsjonalt basert på forbruk (kostbeløp) og forventet kostgjenopprettingsforhold.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet og budsjettsalgsbeløpet angis riktig for hele prosjektet. |
| Løpende |Ført kost = forbruk (kostbeløp)<br /><br /> Ført inntekt = fakturerbar (salgsbeløp) x løpende<br /><br /> Løpende = forbruk (kostbeløp) / budsjett (kostbeløp)<br /> (Refereres til som “Ferdiggjørelsesprosent for kost “ på prosjektoppgavelinjer)<br /><br /> VIA-salg = ført salg - fakturerbar (fakturert pris) |Beregninger av Løpende fører inntekt proporsjonalt basert på prosent fullført, det vil si forbruk (kostbeløp) i forhold til budsjettkost.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet og budsjettkostbeløpet angis riktig for hele prosjektet. |
| Ved avslutning |VIA-beløp = VIA-kostbeløp = Forbruk (kostbeløp)<br /><br /> VIA-salgsbeløp = fakturerbar (fakturert pris) |Ved avslutning fører ikke inntekt og kost før prosjektet er ferdig. Det kan hende du ønsker å gjøre dette når det er stor usikkerhet rundt overslagene for kost og inntekt for prosjektet.<br /><br /> Alt forbruk bokføres i VIA-forbrukskontoen (aktiva), og alt fakturert salg bokføres i VIA-kontoen for fakturert salg (gjeld) til prosjektet er ferdig. |

## <a name="see-also"></a>Se også
[Prosjektstyring](projects-manage-projects.md)  
[Finans](finance.md)  
[Innkjøp](purchasing-manage-purchasing.md)         
[Salg](sales-manage-sales.md)      
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

