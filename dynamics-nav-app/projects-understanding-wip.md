---
title: "Forstå VIA-metoder"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f21357897dd730d96db7abab469d5958c6fe117c
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="understanding-wip-methods"></a>Forstå VIA-metoder

Dynamics NAV støtter metodene nedenfor for å beregne og registrere verdien av varer i arbeid.

|VIA-metode |Beregningsformel |Beskrivelse av beregning|
|-----------|--------------------|-----------------------|
|Kostverdi|Ført inntekt = fakturerbar fakturert pris<br /><br /> Anslått kostbeløp = fakturerbart (salgsbeløp) x budsjett (kostforhold)<br /><br /> VIA-kost = \(løpende - fakturert %\) x anslått kostbeløp<br /><br /> Løpende = forbruk (kostbeløp) / budsjett (kostbeløp)<br /> Fakturert % = fakturerbar (fakturert pris)<br /><br /> Fakturerbar (salgsbeløp) ført kost = forbruk totale kostnader - VIA|Kostverdiberegninger starter med å beregne verdien av det som er oppgitt, ved å ta en andel av anslått kostbeløp basert på prosent fullført. Fakturert kost trekkes fra ved å ta en andel av anslått kostbeløp basert på fakturert prosent.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet, budsjettsalgsbeløpet og budsjettkostbeløpet angis riktig for hele prosjektet.|
|Kostnad for salg|Ført inntekt = fakturerbar fakturert pris<br /><br /> Ført kost = budsjett (kostbeløp) x fakturert prosent<br /><br /> Fakturert % = fakturerbar (fakturert pris) / fakturerbar (salgsbeløp)<br /><br /> \(Fakturert % finnes som en kolonne på prosjektoppgavelinjer\)<br /><br /> VIA-kost = forbruk (kostbeløp) - ført kost|Beregning av solgte varers innkjøps- eller produksjonspris begynner ved å beregne ført kost. Kost føres proporsjonalt basert på budsjettkostbeløp.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet og budsjettkostbeløpet angis riktig for hele prosjektet.|
|Salgsverdi|Ført kost = forbruk (kostbeløp)<br /><br /> Ført inntekt = forbruk (salgsbeløp) x forventet faktureringsforhold<br /><br /> Kostgjenopprettingsprosent = fakturerbar (salgsbeløp) / budsjett (salgsbeløp)<br /><br /> VIA-salg = ført salg - fakturerbar (fakturert pris)|Salgsverdiberegninger fører inntekt proporsjonalt basert på forbruk (kostbeløp) og forventet kostgjenopprettingsforhold.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet og budsjettsalgsbeløpet angis riktig for hele prosjektet.|
|Løpende|Ført kost = forbruk (kostbeløp)<br /><br /> Ført inntekt = fakturerbar (salgsbeløp) x løpende<br /><br /> Løpende = forbruk (kostbeløp) / budsjett (kostbeløp)<br /><br /> \(Refereres til som “Ferdiggjørelsesprosent for kost “ på prosjektoppgavelinjer\)<br /> VIA-salg = ført salg - fakturerbar (fakturert pris)|Beregninger av Løpende fører inntekt proporsjonalt basert på prosent fullført, det vil si forbruk (kostbeløp) i forhold til budsjettkost.<br /><br /> Denne beregningen krever at det fakturerbare salgsbeløpet og budsjettkostbeløpet angis riktig for hele prosjektet.|
|Ved avslutning|VIA-beløp = VIA-kostbeløp = Forbruk \(kostbeløp\)<br /><br /> VIA-salgsbeløp = fakturerbar \(fakturert pris\)|Ved avslutning fører ikke inntekt og kost før prosjektet er ferdig. Det kan hende du ønsker å gjøre dette når det er stor usikkerhet rundt overslagene for kost og inntekt for prosjektet.<br /><br /> Alt forbruk bokføres i VIA-forbrukskontoen \(aktiva\), og alt fakturert salg bokføres i VIA-kontoen for fakturert salg \(gjeld\) til prosjektet er ferdig.|

## <a name="see-also"></a>Se også
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

