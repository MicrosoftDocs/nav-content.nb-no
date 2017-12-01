---
title: Opprette remitteringsforslag
description: "Du kan opprette et remitteringsforslag slik at betalingsforslag sendes til leverandører som skal motta remitteringsoppdrag."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 0d816ef55cd3026bd7bbbc0dbb2f80af069c636c
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-remittance-suggestions"></a>Opprette remitteringsforslag
Du kan opprette et remitteringsforslag slik at betalingsforslag sendes til leverandører som skal motta remitteringsoppdrag. Én betalingstransaksjon per bokføringsdato overføres til banken for hver leverandør.  

> [!NOTE]  
>  Du kan unngå å opprette betalingsforslag for leverandører som remitteres når den ordinære leverandørforslagprosessen benyttes, ved å legge til et filter for **Remittering** i vinduet **Betalingsforslag - leverandør** og sette filteret til **Nei**.  

## <a name="to-create-a-remittance-suggestion"></a>Slik oppretter du et remitteringsforslag:  

1.  Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Betalingskladder**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Remitteringsforslag**.  
3.  Fyll ut feltene som beskrevet i tabellen nedenfor, i hurtigfanen **Alternativer** i vinduet **Remitteringsforslag**.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Siste betalingsdato**|Angi den siste betalingsdatoen.|  
    |**Søk etter kontantrabatter**|Velg dette alternativet hvis du vil søke etter poster med kontantrabatter.|  
    |**Bruk leverandørprioritet**|Velg dette alternativet hvis leverandørprioritet skal brukes til å søke i poster.|  
    |**Disponibelt beløp (NOK)**|Angi betalingene for totalsummer som er mindre enn eller lik det angitte beløpet.|  
    |**Bokføringsdato**|Angi en bokføringsdato.|  
    |**Erstatt bokføringsdato med forfallsdato**|Velg for å sette inn forfallsdatoen for posten som bokføringsdato for betalingene.|  
    |**Sjekk bilagstype**|Angi hvilke av følgende bilagstyper som skal sjekkes for betaling:<br /><br /> -   **Alle** - alle bilagstyper sjekkes.<br />-   **Faktura/kreditnota** - Bare faktura- eller kreditnotaposter sjekkes.|  
    |**Bare faktura-/debetposter**|Velg dette for å bare betale faktura- eller debetposter.|  

4.  Velg **OK**.  

## <a name="see-also"></a>Se også  
 [Elektroniske betalinger til leverandører i Norge](electronic-payments-to-vendors-in-norway.md)   
 [Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md)   
 [Opprette remitteringskontoer](how-to-create-remittance-accounts.md)   
 [Angi leverandører for remittering](how-to-set-up-vendors-for-remittance.md)   
 [Mottakerreferansekoder](recipient-reference-codes.md)   
 [Opprette manuelle remitteringsoppdrag](how-to-create-manual-remittance-payments.md)   
 [Definere betalingslinjeinformasjon](how-to-set-up-payment-line-information.md)   
 [Kontrollere remitteringsoppdrag](how-to-test-remittance-payments.md)   
 [Eksportere remitteringsoppdrag](how-to-export-remittance-payments.md)   
 [Typer betalingsreturfiler](types-of-payment-returns-files.md)   
 [Importere betalingsreturdata](how-to-import-payment-return-data.md)   
 [Slette remitteringsoppdrag](how-to-delete-remittance-payment-orders.md)   
 [Remitteringsfeil](remittance-errors.md)   
 [Vise remitteringsfeilkoder](how-to-view-remittance-error-codes.md)   
 [Annullere betalinger](how-to-cancel-payments.md)

