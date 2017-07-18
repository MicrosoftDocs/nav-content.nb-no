---
title: Mva- og mva-grupper i USA og Canada
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Mva- og mva-grupper i USA og Canada
Når du begynner å bruke Dynamics NAV, kan du kjøre en assistert installasjonsveiledningen for hurtig og enkelt sette opp mva-informasjon for firmaet, og eventuelt for kundene og leverandørene. I løpet av minutter er du klar til å opprette salgsdokumenter og kjøpsdokumenter med riktig beregnet merverdiavgift.
Hvis du flytter til det tomme Mitt firma, anbefaler vi at du starter med å bruke hver av de assisterte installasjonsveiledningene, inkludert den for mva. Hvis du foretrekker å definere mva selv, vil denne artikkelen forklarer hva du må ta hensyn til.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Mva-grupper, mva-områder og mva-jurisdiksjoner
I Dynamics NAV representerer en mva-gruppe en gruppe av lagervarer eller ressurser som det skal beregnes like mye mva. av. Ikke i Norge. Du kan for eksempel angi en mva-gruppe for avgiftspliktige varer og en annen for ikke-avgiftspliktige varer. Du må tilordne mva-gruppekoder til varer og finanskonti. Du må også tilordne mva-områdekoder til kunder, lokasjoner og til dine egne firmainnstillinger. Den assisterte installasjonsveiledningen hjelper deg med å gjøre dette.  

Hver enkelt mva-område er en gruppering av mva-jurisdiksjoner som er basert på en bestemt geografisk lokasjon. Mva-området for Miami i Florida, inneholder for eksempel tre mva-jurisdiksjoner: by (Miami), fylke (Dade), og delstat (Florida). Dynamics NAV inneholder et begrenset sett med mva-områder med en standardkonfigurasjon, men du kan endre dem og legge til nye mva-områder.  

Hvis du konfigurerer nye mva-områder og mva-jurisdiksjoner, må du forsikre deg om at du fyller ut feltene på riktig måte. I USA kan delstater, fylker, byer og lokasjoner kreve mva. I Canada kan føderale myndigheter og provinser kreve mva. Firmaer samler inn og remitterer mva til disse myndighetene for produkter som selges til sluttbrukere. Mva kan også kreves på eksisterende mva. Mva kan for eksempel beregnes for en salgsfaktura som allerede inkluderer mva fra andre jurisdiksjoner.  

I Canada må mva-beløp være angitt i dokumenter for hver mva-jurisdiksjon. Opptil fire jurisdiksjoner kan vises i et dokument, og jurisdiksjoner som har samme utskriftsrekkefølgen kombineres når de skrives ut.

## <a name="tax-details"></a>Mva-detaljer
Vinduet **Mva-detaljer** viser forskjellige kombinasjoner av mva-jurisdiksjoner og mva-grupper for å opprette mva-satser. For hver mva-jurisdiksjon anbefaler vi at du definerer en mva-gruppe for vanlig mva, en annen mva-gruppe for varer eller tjenester som ikke er mva-belagt og en ekstra mva-gruppe for hver vare eller tjeneste som er behandlet med en annen mva-sats i denne jurisdiksjonen.  

I USA, når du selger til en kunde på en lokasjon der du ikke har en *situs*, eller en juridisk lokasjon i denne delstaten, krever du ikke inn mva. For lokasjoner der du ikke har en juridisk lokasjon må du sikre at feltene **Mva. under maksimum** og **Mva. over maksimum** er 0,00.  

## <a name="see-also"></a>Se også
[Finans](finance-setup.md)  
[Konfigurere finans](finance-setup-setup-finance-setup.md)  
[Mva og avgifter for varer og tjenester i USA og Canada](ca-finance-setup-tax.md)  
[Enkelt oppsett av mva](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  

