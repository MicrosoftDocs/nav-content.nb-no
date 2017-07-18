---
title: Registrere forbruk for prosjekter
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
ms.openlocfilehash: 86cc31ea9c117700d2905dd6b8c4bd88eb0f9854
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-usage-for-jobs"></a>Registrere forbruk for prosjekter
I vinduet **Prosjektplanleggingslinjer** kan du gå gjennom og registrere forbruk i ulike deler av prosjektet, som oppdateres automatisk når du endrer og overfører informasjon mellom prosjekter og prosjektkladder eller prosjektfakturaer. Dette krever at du har satt opp et prosjekt slik at **Bruk forbrukskobling** er aktivert. Se [Sette opp prosjekter](projects-how-setup-jobs.md) for mer informasjon.  

For planleggingslinjer av typen **Budsjett** kan du for eksempel angi antallet for en ressurs og antallet som skal overføres til prosjektkladden. Hvis planleggingslinjetypen er **Fakturerbar**, kan du angi antallet for ressursen og angi antallet som skal overføres til en faktura. Ved å sammenligne antallet som er overført til kladden eller fakturaen, med det gjenstående antallet kan du raskt se gjennom informasjon om forbruk.

De følgende fremgangsmåtene viser hvordan du registrerer faktiske (fakturerbare) eller budsjetterte prosjektpriser og -kostnader. Hvis du vil ha informasjon om estimering av budsjetterte verdier under planleggingen, kan du se [Administrere prosjektbudsjetter](projects-how-manage-budgets.md).

## <a name="to-record-usage-for-a-job-planning-line-of-type-budget"></a>Slik registrerer du forbruk for en prosjektplanleggingslinje av typen Budsjett

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Velg det aktuelle prosjektet, og velg deretter handlingen **Prosjektplanleggingslinjer**.
3. Velg en prosjektplanleggingslinje av typen **Budsjett** eller **Både Budsjett og fakturerbar** som du vil registrere forbruk for.
4. Angi antallet du vil overføre til fakturaen, i feltet **Ant. som skal overføres til kladd**. Standardantallet er verdien du angir i feltet **Antall**.

    Feltet **Restantall** viser antallet som gjenstår for å fullføre prosjektet og overføres til kladden.  

5. Velg handlingen **Opprett prosjektkladdelinjer**.
6. I vinduet **Prosjekt – overfør til prosjektplanleggingslinje** fyller du ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
7. Velg handlingen **Åpne prosjektkladd**.  
8. I vinduet **Prosjektkladd** velger du den relevante linjen, og deretter velger du handlingen **Bokfør**.
9. I vinduet **Prosjektplanleggingslinjer** går du gjennom det registrerte forbruket ved å kontrollere feltene **Antall**, **Restantall** og **Ant. som skal overføres til kladd**.  
10. Gjenta trinn 3 til 8 for å registrere ekstra forbruk.  

## <a name="to-record-usage-for-a-job-planning-line-of-type-billable"></a>Slik registrerer du forbruk for en prosjektplanleggingslinje av typen Fakturerbar  
I den neste oppgaven registrerer du også forbruk, men for en prosjektplanleggingslinje av typen **Fakturerbar**. I dette tilfellet fakturerer du vanligvis forbruket, men du kan også overføre det til kladden. Når du gjør dette, opprettes imidlertid en prosjektplanleggingslinje av typen **Budsjett** for å samsvare med den fakturerbare linjen. Hvis du vil ha mer informasjon, se [Administrere prosjektbudsjetter](projects-how-manage-budgets.md).

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.
2. Velg det aktuelle prosjektet, og velg deretter handlingen **Prosjektplanleggingslinjer**.  
3. Velg en prosjektplanleggingslinje av typen **Fakturerbar** som du vil registrere forbruk for.
4. Angi antallet du vil overføre til fakturaen, i feltet **Ant. som skal overføres til faktura**. Standardantallet er verdien du angir i feltet **Antall**.

    Feltet **Antall å fakturere** viser antallet som gjenstår for å fullføre prosjektet og faktureres.  

5. Velg handlingen **Opprett salgsfaktura**.
6. I vinduet **Prosjekt – overfør til salgsfaktura** fyller du ut feltene etter behov, og deretter velger du **OK**-knappen.
7. I vinduet **Prosjektplanleggingslinjer** velger du den relevante linjen, og deretter velger du handlingen **Bokfør**.
8. Se gjennom det registrerte forbruket ved å kontrollere feltene **Antall**, **Antall som skal faktureres** og **Ant. som skal overføres til faktura**, og hvis salgsfakturaen er bokført, feltet **Ant. fakturert**.
9. Gjenta trinn 3 til 8 for å registrere ekstra forbruk.  
10. Hvis du vil gå gjennom en relatert bokført salgsfaktura, velger du handlingen **Salgsfakturaer/kreditnotaer**.  
11. Velg den aktuelle fakturaen i vinduet **Prosjektfakturaer**, og velg deretter handlingen **Åpne salgsfaktura/kreditnota**.         

## <a name="to-create-job-journal-lines-from-job-planning-lines"></a>Slik oppretter du prosjektkladdelinjer fra prosjektplanleggingslinjer:  
Når du er klar til å bokføre finansinformasjon for prosjekter, må du opprette prosjektkladdelinjene som du kan bokføre.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Velg et aktuelt åpent prosjekt, og velg deretter handlingen **Prosjektplanleggingslinjer**.  
3. I vinduet **Prosjektplanleggingslinjer** på en relevant prosjektplanleggingslinje angir du antallet du vil overføre til en prosjektkladd, i feltet **Ant. som skal overføres til kladd**.  
4. Velg handlingen **Opprett prosjektkladdelinjer**.
5. I vinduet **Prosjekt – overfør til prosjektplanleggingslinje** fyller du ut feltene etter behov.  
6. Velg **OK**-knappen. Prosjektkladdelinjer opprettes.
7. Hvis du vil bekrefte overføringen, åpner du den aktuelle prosjektkladden og kontrollerer postene.  
8. Når prosjektkladdelinjene er fullført, kan du velge handlingen **Bokfør**.  

## <a name="to-create-job-journal-lines-manually"></a>Slik oppretter du prosjektkladdelinjer manuelt:  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjektkladder** og velger deretter den relaterte koblingen.  
2. Velg et navn for den relevante prosjektkladden i feltet **Bunkenavn**.  
3. Angi bilagsnummer, prosjektnummer, prosjektoppgavenummer, type og antall for typen som forbrukes, på en ny linje.  
4. Når prosjektkladdelinjene er fullført, kan du velge handlingen **Bokfør**.  

## <a name="to-review-planning-lines-for-a-job-ledger-entry"></a>Slik går du gjennom planleggingslinjene for en prosjektpost  
Etter at du har bokført prosjektkladdelinjer kan du vise planleggingslinjene som er knyttet til prosjektpostene som er bokført.

**Merk**: Dette krever at det er merket av for **Bruk forbrukskobling** for prosjektet, eller at dette er standardinnstillingen for alle prosjekter i organisasjonen. Se [Sette opp prosjekter](projects-how-setup-jobs.md) for mer informasjon.  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjektkladder** og velger deretter den relaterte koblingen.  
2. Velg en kladd for det aktuelle prosjektet, og velg deretter handlingen **Poster**.  
3. I vinduet **Prosjektposter** velger du handlingen **Vis koblede prosjektplanleggingslinjer**.

## <a name="see-also"></a>Se også
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

