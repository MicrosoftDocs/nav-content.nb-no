---
title: Bekrefte organisasjonsnumre
description: "Du kan bruke en EU-webtjeneste til å bekrefte at organisasjonsnumre du angir på kunde-, leverandør- eller kontaktkort, er gyldige."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8ed345e346ba32a38ebb2738afbe6c12749842ff
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-verify-vat-registration-numbers"></a>Bekrefte organisasjonsnumre
Du kan bruke en EU-webtjeneste til å bekrefte at organisasjonsnumre du angir på kunde-, leverandør- eller kontaktkort, er gyldige.  

 Når du endrer feltet **Organisasjonsnummer** på et kort der verdien i feltet **Lands-/regionskode** er et EU-land/område, logges det nye organisasjonsnummeret og bruker-ID-en din i vinduet **Organisasjonsnummerlogg**. Du bekrefter et organisasjonsnummer ved å klikke knappen **Bekreft registreringsnummer** i vinduet **Organisasjonsnummerlogg**. Det opprettes en ny linje hver gang du bruker funksjonen for bekreftelse. Hvis nummeret kan bekreftes, inneholder **Status**-feltet **Gyldig**. Hvis nummeret ikke kan bekreftes, inneholder **Status**-feltet **Ugyldig**, og du må deretter endre nummeret i **Organisasjonsnummer**-feltet på kortet og starte funksjonen for bekreftelse på nytt.  

 Nettadressen for standard webtjeneste er definert i feltet **URL-adresse for validering av organisasjonsnummer** i vinduet **Finansoppsett**.  

 I tabellen **Format for organisasjonsnr.** kan du endre de ulike formatene for organisasjonsnummer som brukerne kan angi i feltet **Organisasjonsnr.**, for hvert landregion.  

> [!WARNING]  
>  Denne webtjenesten bruker HTTP-protokollen, som betyr at data som overføres via tjenesten, ikke er kryptert.  

> [!NOTE]  
>  Denne tjenesten er en del av et omfattende EU-nettverk av nasjonale mva-registre, og du kan oppleve nedetid som Microsoft ikke er ansvarlig for.  

## <a name="to-verify-a-vat-registration-number-from-a-customer-card"></a>Slik bekrefter du et organisasjonsnummer fra et kundekort:  
Nedenfor beskrives hvordan du bekrefter et organisasjonsnummer for en kunde. Trinnene er de samme for en leverandør og en kontakt.   
1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kunder**, og velg deretter den relaterte koblingen.  

2.  Åpne kortet til en kunde der du vil bekrefte organisasjonsnummeret.  

    > [!NOTE]  
    >  Feltet **Lands-områdekode** på kundekortet må inneholde EU-land-område.  
3.  Velg DrillDown-knappen ved siden av **Organisasjonsnr.**-feltet i hurtigfanen **Fakturering**.  

    Vinduet **Organisasjonsnummerlogg** åpnes og viser én linje der **Status**-feltet inneholder **Ikke bekreftet**.  
4.  Velg handlingen **Bekreft registreringsnummer**.  

     Det opprettes en ny linje der **Status**-feltet inneholder enten **Gyldig** eller **Ugyldig**.  
5.  Hvis **Status**-feltet inneholder **Ugyldig**, endrer du nummeret i **Organisasjonsnummer**-feltet på kortet, og deretter gjentar du trinn 3 og 4.  

## <a name="see-also"></a>Se også  
[Finans](finance.md)  
[Registrere nye kunder](sales-how-register-new-customers.md)  
[Registrere nye leverandører](purchasing-how-register-new-vendors.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

