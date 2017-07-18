---
title: Administrere prosjektforsyninger
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
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a>Administrere prosjektforsyninger
Behandling av prosjektforsyninger som varer, tjenester og utgifter inngår i og er en viktig del av alle prosjektutførelser. Du kan bruke lagerantallene eller foreta prosjektspesifikke kjøp ved hjelp av bestillinger eller kjøpsfakturaer. En servicejobb på en datamaskin krever for eksempel en ny disk. Du oppretter en kjøpsfaktura for å kjøpe en ny disk, og registrerer prosjektet den skal brukes på.

Hvis kjøpsprosessen ikke krever at den fysiske transaksjonen registreres separat, kan et kjøp behandles i vinduet **Finanskladd for prosjekt**. Hvis du vil ha mer informasjon, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).

## <a name="to-purchase-items-or-services-for-a-job"></a>Slik kjøper du varer eller tjenester for et prosjekt
Følgende fremgangsmåte viser hvordan du bruker en kjøpsfaktura til å kjøpe produkter for et prosjekt. Bruk samme fremgangsmåte når du bruker en bestilling.  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kjøpsfakturaer** og velger deretter den relaterte koblingen.  
2. Velg handlingen **Nytt** og fyll ut feltene etter behov. Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md).
3. I feltene **Prosjektnr.** og **Prosjektoppgavenr.** velger du informasjonen på prosjektet som du vil kjøpe varer eller tjenester for.  

    Verdien du velger i feltet **Prosjektlinjetype**, definerer om en planleggingslinje blir opprettet når du bokfører forbruket for varen. Hvis feltet inneholder **Fakturerbar**, opprettes det prosjektplanleggingslinjer som er klare for å faktureres kunden. Hvis du vil ha mer informasjon, kan du se [Fakturere prosjekter](projects-how-invoice-jobs.md).

4. Velg handlingen **Bokfør**.

## <a name="to-view-the-value-of-purchases-for-a-job"></a>Slik viser du verdien av kjøp for et prosjekt  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.
2. Åpne et aktuelt prosjektkort.

    På hurtigfanen **Oppgaver** viser feltet **Utestående bestillinger** det totale utestående beløpet, i lokal valuta, for lagervarer og tjenester i kjøpsdokumenter for prosjektoppgavelinjen.  

    Feltet **Mottatt, ikke fakturert (beløp)** viser verdien for varer som er levert i kjøpsdokumenter, men som ennå ikke er fakturert.  

3. Velg enten feltene for å åpne vinduet **Bestillingslinjer**, der du kan gå gjennom informasjon om de relaterte kjøpsdokumentlinjene, inkludert hvilke varer eller tjenester som er mottatt.

## <a name="to-post-a-job-related-expense"></a>Slik bokfører du en prosjektrelatert utgift  
Hvis du pådrar deg ekstraordinære eller enkeltstående prosjektutgifter, kan du bruke vinduet **Finanskladd for prosjekt** til å bokføre dem direkte til den aktuelle prosjektkontoen.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladder for prosjekt** og velger deretter den relaterte koblingen.  
2. Opprett en ny linje, og skriv inn informasjon om utgiften, inkludert informasjon i feltene **Prosjektnr.** og **Prosjektoppgavenr.**  
3. Når kladden er fullført, kan du velge handlingen **Bokfør**.


## <a name="see-also"></a>Se også
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

