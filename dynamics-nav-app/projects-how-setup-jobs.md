---
title: Konfigurere prosjekter
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
ms.openlocfilehash: ce9c980caf73a36b3e2c7d07141b096fcff06590
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-jobs"></a>Konfigurere prosjekter
I vinduet **Prosjektoppsett** må du angi hvordan du vil bruke bestemte prosjektfunksjoner.

Du må sette opp priser for prosjektvarer, prosjektressurser og finanskonti på individuelle prosjektkort, og må du definere prosjektbokføringsgrupper.

## <a name="to-set-general-information-for-jobs"></a>Slik angir du generell informasjon for prosjekter
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjektoppsett** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

**Merk**: Avmerkingsboksen **Bruk forbrukskobling** er ganske komplisert, og derfor er forklart i delen nedenfor.

## <a name="to-set-up-job-usage-tracking"></a>Slik konfigurerer du sporing av prosjektforbruk
Når du kjører en jobb, vil du kanskje vite hvordan din bruk spores mot planen din. Du kan enkelt gjøre dette ved å opprette en kobling mellom jobbplanleggingslinjene og det faktiske forbruket. Dette lar deg spore kostnader og enkelt se hvor mye arbeid som gjenstår. Som standard er prosjektplanleggingslinjetypen **Budsjett**, men bruk av linjetypen **Både Budsjett og Fakturerbar** har liknende effekter.

Hvis du merker av for **Bruk forbrukskobling**, kan du se gjennom informasjon om prosjektplanleggingslinjen. Du kan angi antallet for ressursen, varen eller finanskontoen og deretter angi antallet du vil overføre til prosjektkladden. Feltet **Restantall** på prosjektplanleggingslinjen angir det som gjenstår å overføres og bokføres til prosjektkladden.

Når det er merket av for **Bruk forbrukskobling** og prosjektplanleggingslinjetypen er **Fakturerbar**, oppretter Finans en prosjektplanleggingslinjer av typen **Budsjett** etter at du bokfører kladdelinjen.

**Merk**: Hvis det er merket av for **Bruk forbrukskobling** på prosjektkortet og feltet **Linjetype** på prosjektkladdelinjen er tomt, opprettes det nye prosjektplanleggingstyper av linjetypen **Budsjett** når du bokfører prosjektkladdelinjer. Hvis det ikke er merket av for **Bruk forbrukskobling** på prosjektkortet og feltet **Linjetype** på prosjektkortet er tomt, opprettes det ingen prosjektplanleggingslinjer når du bokfører prosjektkladdelinjer. Hvis du vil ha mer informasjon, kan du se [Registrere forbruk for prosjekter](projects-how-record-job-usage.md).

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjektoppsett** og velger deretter den relaterte koblingen.
2. Merk av for eller fjern merket for **Bruk forbrukskobling**.

**Merk**: Du kan angi en annen innstilling for avmerkingsboksen **Bruk forbrukskobling** på hvert prosjektkort. I slike tilfeller overstyrer innstillingen for dette prosjektet den generelle standarden som er beskrevet ovenfor.

## <a name="to-set-up-prices-for-job-resources"></a>Slik konfigurerer du priser for prosjektressurser  
Du kan definere bestemte priser for ressurser for et prosjekt. Du bruker vinduet **Ressurspriser for prosjekt** til å gjøre dette.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Velg det aktuelle prosjektet, og velg deretter handlingen **Ressurs**.
3. Fyll ut feltene etter behov i vinduet **Ressurspriser for prosjekt**.

Den valgfrie informasjonen i feltene **Prosjektoppgavenr.**, **Arbeidstype**, **Valutakode**, **Linjerabatt-%** og **Enhetskostfaktor** blir brukt på prosjektplanleggingslinjene og i forbrukskladdene når denne ressursen angis og legges til i prosjektet.  

Verdien i feltet **Salgspris** for ressursen blir brukt på prosjektplanleggingslinjene og i prosjektkladder når du angir denne ressursen, en ressurs som er tilordnet ressursgruppen, eller en hvilken som helst ressurs.  

**Merk**: Denne prisen overstyrer alltid eventuelle priser som er definert i det eksisterende vinduet **Ressurspris/Ressursgruppepriser**.

## <a name="to-set-up-prices-for-job-items"></a>Slik konfigurerer du priser for prosjektvarer  
Du kan definere bestemte priser for varer for et prosjekt. Du bruker vinduet **Varepriser for prosjekt** til å gjøre dette.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Velg det aktuelle prosjektet, og velg deretter handlingen **Vare**.
3. Fyll ut feltene etter behov i vinduet **Varepriser for prosjekt**.

Den valgfrie informasjonen i feltene **Prosjektoppgavenr.**, **Valutakode** og **Linjerabatt-%** blir brukt på prosjektplanleggingslinjene og prosjektkladdene når denne varen angis og legges til i prosjektet.  

Verdien i feltet **Salgspris** for varen blir brukt på prosjektplanleggingslinjene og i prosjektkladder når du angir denne varen.  

**Merk**: Denne prisen overstyrer alltid den vanlige kundeprisen (funksjonen for "beste pris") for varer. Hvis du vil bruke de vanlige kundeprismekanismene, må du ikke opprette prosjektvarepriser for prosjektet.

## <a name="to-set-up-prices-for-job-general-ledger-accounts"></a>Slik setter du opp priser for prosjektfinanskonti  
Du kan definere bestemte priser for finansutgifter for et prosjekt. Du bruker vinduet **Finanskontopriser for prosjekt** til å gjøre dette.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Prosjekter** og velger deretter den relaterte koblingen.  
2. Velg det aktuelle prosjektet, og velg deretter handlingen **Finanskonto**.  
3. Fyll ut feltene etter behov i vinduet **Finanskontopriser for prosjekt**.

Den valgfrie informasjonen i feltene **Prosjektoppgavenr.**, **Arbeidstype**, **Valutakode**, **Linjerabatt-%** og **Enhetskost** blir brukt på prosjektplanleggingslinjene og i prosjektkladdene når denne finanskontoen angis og legges til i et prosjekt.  

Verdien i feltet **Salgspris** for finansprosjektutgiften blir brukt på prosjektplanleggingslinjene og i prosjektkladder når denne finanskontoen angis.

## <a name="to-set-up-job-posting-groups"></a>Slik definerer du prosjektbokføringsgrupper  
Ett aspekt ved prosjektplanlegging er å bestemme hvilke bokføringskontoer som skal brukes for prosjektkostnader. Du må definere konti for bokføring for hver prosjektbokføringsgruppe for å kunne bokføre prosjekter. En bokføringsgruppe representerer en kobling mellom jobben og hvordan den skal behandles i finans. Når du oppretter en jobb, angir du en bokføringsgruppe, og hver oppgave du oppretter for prosjektet, knyttes som standard til denne bokføringsgruppen. Når du oppretter oppgaver, kan du imidlertid overstyre standardinnstillingen og velge en bokføringsgruppe som er mer hensiktsmessig.  

**Merk**: De nødvendige kontiene i kontoplanen må konfigureres før du definerer bokføringsgrupper. Hvis du vil ha mer informasjon, se [Definere eller endre kontoplanen](finance-setup-setup-chart-accounts.md).  

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokføringsgrupper - prosjekt** og velger deretter den relaterte koblingen.  
2. Velg handlingen **Ny** og fyll deretter ut kontofeltene som beskrevet i tabellen nedenfor.  

|Kontofelt|Beskrivelse|
|-------------|-----------|
|**Kode**|En kode for bokføringsgruppen. Du kan angi opptil 10 tegn, medregnet mellomrom.|  
|**VIA-forbrukskonto**|VIA-kontoen for beregnet kost for VIA for prosjekt. Dette er en balansekonto for kapitalaktiva.|
|**VIA-salgskonto**|En konto for metoden Kostverdi eller Kostnad for salg i VIA-beregning, som er en gjeldskonto for påløpte utgifter i balansen. Det bokføres til denne når VIA-justeringen krever at forbrukskostbeløpene som bokføres i resultatregnskapet, økes.|  
|**Forbrukskonto (resultat) for prosjekt**|En motkonto for VIA-forbrukskontoen. Dette er en motkonto for negativ utgift.|
|**Konto for utlignede varekostnader**|En motkonto for VIA-forbrukskontoen. Dette er en motkonto for negativ utgift.|
|**Konto for utlignede ressurskostnader**|En motkonto for VIA-forbrukskontoen. Dette er en motkonto for negativ utgift.|
|**Forbrukskonto (resultat)**|En motkonto for VIA-forbrukskontoen. Dette er en motkonto for negativ utgift.|
|**Salgskonto for prosjekt**|Motkontoen for VIA-salgskontoen. Dette er en utgiftskonto.|
|**Salgsutgiftskonto (budjett)**|Salgskontoen som skal brukes til finansutgifter i prosjektoppgaver med denne bokføringsgruppen. Hvis du lar dette feltet stå tomt, brukes finanskontoen som er angitt på prosjektplanleggingslinjen.|
|**VIA-konto for påløpt salg**|VIA-kontoen for beregnet salgsverdi for VIA for prosjekt. Dette er en balansekonto for påløpt inntekt. Det bokføres på denne når VIA-justeringen krever at ført inntekt skal økes.|
|**VIA-konto for fakturert salg**|Kontoen for den fakturerte salgsverdien for VIA som ikke kan føres. Dette er en balanse for ikke tjent inntekt.|
|**Konto for utlignet salg for prosjekt**|Motkontoen for VIA-kontoen for fakturert salg. Dette er en motkonto for inntekt.|
|**Salgsjusteringskonto for prosjekt**|Motkontoen for VIA-prosjektsalgskontoen. Dette er en inntektskonto.|
|**Konto for ført kost**|Utgiftskontoen som inneholder de førte kostbeløpene for prosjektet. Dette er som regel en debitutgiftskonto.|
|**Konto for ført salg**|Inntektskontoen som inneholder ført inntekt for prosjektet. Dette er som regel en kreditinntektskonto.|

## <a name="see-also"></a>Se også
[Konfigurere prosjektstyring](projects-setup-projects.md)  
[Administrere prosjekter](projects-manage-projects.md)  
[Finans](finance-setup.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)         
[Håndtere salg](sales-manage-sales.md)      
[Arbeide med Dynamics NAV](ui-work-product.md)  

