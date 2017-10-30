---
title: Definere SEPA Direct Debit
description: "Lær hvordan du definerer SEPA Direct Debit i Dynamics NAV"
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: b768f78cd8ef7f6981e5e148fee5f61e9ab922ee
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-sepa-direct-debit"></a>Definere SEPA Direct Debit
Fra **Direct Debit-oppkrevinger**-vinduet kan du eksportere instruksjoner til den elektroniske banken for å utføre en direct debit-samling fra kundens bankkonto til din bankkonto. [!INCLUDE[d365fin](includes/d365fin_md.md)] støtter formatet for SEPA Direct Debit, men andre formater for elektroniske betalinger kan være tilgjengelige i ditt land/region.  

Du kan gjøre det mulig å eksportere et bankfilformat som ikke støttes som standard i [!INCLUDE[d365fin](includes/d365fin_md.md)], ved å definere en datautvekslingsdefinisjon ved hjelp av rammeverket for datautveksling. Hvis du vil ha mer informasjon om oppsett, kan du se [Definere datautvekslingsdefinisjoner](across-how-to-set-up-data-exchange-definitions.md)  

Før du kan behandle kundebetalinger elektronisk ved å eksportere direct debit-instruksjoner i SEPA Direct Debit-formatet, må du utføre følgende konfigureringstrinn:  

* Konfigurer eksportformatet for bankfilen som instruerer banken om å utføre en direct debit-samling fra kundens bankkonto til din bankkonto.  
* Konfigurer kundens betalingsmåte.  
* Konfigurer direct debit-belastningsfullmakten som gjenspeiler avtalen med kunden om å samle sine betalinger i en bestemt avtaleperiode.  

### <a name="to-set-up-your-bank-account-for-sepa-direct-debit"></a>Slik konfigurerer du din bankkonto for SEPA direct debit  
1. Skriv inn **Bankkontoer** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
2. Åpne bankkontoen som du vil bruke til direct debit.  
3. Velg alternativet for SEPA direct debit i feltet **Eksportformat for SEPA Direct Debit** i hurtigfanen **Overfør**.  

### <a name="to-set-up-the-customers-payment-method-for-sepa-direct-debit"></a>Slik konfigurerer du kundens betalingsmåte for SEPA direct debit  
1. Skriv inn **Betalingsmåter** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
2. Velg handlingen **Ny**.  
3. Konfigurer betalingsmåter. Fyll ut de spesifikke feltene for direct\- debit som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Direct Debit**|Angi om betalingsmåten er for SEPA direct debit-samlinger.|  
    |**Betalingsbet.kode for Direct Debit**|Angi betalingsbetingelsene, for eksempel IKKE BETAL, som vises på salgsfakturaer som betales med SEPA direct debit, for å angi for kunden at betalingen blir innkrevd automatisk. Du kan også la feltet stå tomt.|  

    > [!NOTE]  
    >  Ikke angi en verdi i feltet **Motkontonr.**  

4. Velg **OK**-knappen for å lukke vinduet **Betalingsmåter**.  
5. Skriv inn **Kunder** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
6. Åpne kundekortet for kunden som du vil konfigurere SEPA direct debit-samling for.  
7. Velg feltet **Betalingsmåte - kode**, og velg deretter koden for betalingsmåte som du angav i trinn 3.  
8. Gjenta trinn 6 og 7 for alle kundene du vil konfigurere SEPA direct debit-samling for.  

#### <a name="to-set-up-the-direct-debit-mandate-that-represents-the-customer-agreement"></a>Slik konfigurerer du direct debit-belastningsfullmakten som representerer kundeavtalen  
1. Skriv inn **Kunder** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
2. Åpne kortet for kunden som du vil konfigurere SEPA direct debit for.  
3. Velg **Bankkonti**-handlingen.  
4. I vinduet **Kundebankkonto - oversikt** velger du kundebankkonto som skal bruke direct debit, og deretter velger du **Direct Debit-belastningsfullmakter** i **Prosess**-gruppen i kategorien **Hjem**.  
5. I vinduet **SEPA Direct Debit-belastningsfullmakter** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Bankkontokode for kunde**|Angir bankkontoen som avtale\-girobetalinger kreves inn fra. Dette feltet fylles ut automatisk.|  
    |**Gyldig fra**|Angi datoen direct debit\-belastningsfullmakten gjelder fra.|  
    |**Gyldig til**|Angi datoen da direct debit\-belastningsfullmakten utløper.|  
    |**Signeringsdato**|Angi datoen da kunden signert direct debit\-belastningsfullmakten.|  
    |**Type betaling**|Angi om avtalen dekker flere (**Gjentakende**) eller én enkelt (**Engangsforekomst**) direct debit-samlinger.|  
    |**Forventet antall debetbeløp**|Angi hvor mange direct debit-samlinger vil opprette. Dette feltet er bare relevant hvis du valgte **Gjentakende** i feltet **Type betaling**.|  
    |**Debetteller**|Angir hvor mange direct debit-samlinger som er utført ved hjelp av denne direct debit\-belastningsfullmakten. Dette feltet oppdateres automatisk.|  
    |**Sperret**|Angi om direct debit-samlinger ikke kan opprettes ved hjelp av denne direct debit\-belastningsfullmakten.|  

6.  Gjenta trinn 1 til 5 for alle kundene du vil konfigurere SEPA direct debit for.  

 Direct debitbelastningsfullmakten fylles automatisk ut i feltet **ID for Direct Debit-belastningsfullmakt** når du oppretter en salgsfaktura for kunden som du valgte i trinn 2. Hvis du vil ha mer informasjon, se [Opprette gjentakende salgs- og kjøpslinjer](sales-how-work-standard-lines.md).  

## <a name="see-also"></a>Se også  
[Innkreve betalinger med SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)  
[Definere datautvekslingsdefinisjoner](across-how-to-set-up-data-exchange-definitions.md)
[Opprette gjentakende salgs- og kjøpslinjer](sales-how-work-standard-lines.md)
[Utveksle data elektronisk](across-data-exchange.md)

