---
title: Opprette remitteringskontoer
description: "Du må opprette én remitteringskonto for hver bankkonto hvor betaling utføres."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 7b00ceb7bb37a1ebecece22b69e53b9cd61ea65f
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-create-remittance-accounts"></a>Opprette remitteringskontoer
Du må opprette én remitteringskonto for hver bankkonto hvor betaling utføres. Hvis en konto brukes til å utføre betalinger til både innenlandske og utenlandske leverandører, må denne kontoen opprettes to ganger: én gang for betalinger innland og én gang for betalinger utland.  

> [!NOTE]  
>  Valutaen som brukes for bankkontoen skal være samme valuta som banken bruker for denne kontoen. Valutakursene er basert på kontoens valuta og beregningene er basert på denne valutaen.  

## <a name="to-create-a-remittance-account"></a>Slik oppretter du en remitteringskonto  

1.  Velg ikonet ![Søk etter side eller rapport](../../media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Remitteringskontooversikt**, og velg deretter den relaterte koblingen.  
2.  Velg handlingen **Ny**.  
3.  Fyll ut feltene som beskrevet i tabellen nedenfor, i hurtigfanen **Generelt** i vinduet **Remitteringskontokort**.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Kode**|Angi identifikasjonskoden for kontoen.|  
    |**Remitteringsavtalekode**|Velg avtalen som kontoen er knyttet til.|  
    |**Type**|Velg betalingstypen. Betalingstyper omfatter **Innland**, **Utland**, og **Bet. Inst.**.<br /><br /> Ved remittering til Bankenes Betalingssentral (BBS) kan du bare velge **Innland**.|  
    |**Beskrivelse**|Angir beskrivelsen av kontoen.|  
    |**Bankkontonr.**|Angi kontonummeret for banken.|  
    |**BBS Avtale ID**|Angi avtale-ID-en for hver konto i BBS.|  

4.  I hurtigfanen **Finans** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Kontotype**|Velg kontotypen. Kontotyper inkluderer **Finanskonto** og **Bankkonto**.|  
    |**Kontonr.**|Angi kontonummeret avhengig av hva du valgte i feltet **Kontotype**.|  
    |**Gebyrkontonr.**|Angi kontonummeret for gebyrkontoen.|  
    |**Avrunding/Avvikkontonr.**|Angi finanskontoen for å bokføre avviket som et resultat av avrunding.|  
    |**Maks. avrunding/avvik (NOK)**|Angi den maksimale avrundingen eller det maksimale avviket som godtas av avregningsreturen.|  
    |**Bilagsnr.serie**|Angi nummerserien som skal brukes når du bokfører betalinger ved hjelp av remitteringssystemet.|  
    |**Nytt bilag pr.**|Velg hvordan bilagene skal nummereres når du bokfører en betaling:<br /><br /> -   **Dato** - Nye bilag nummereres i henhold til datoen for når betalingen utføres.<br />-   **Leverandør** - Nye bilag nummereres i henhold til leverandør.|  
    |**Returkladd malnavn**|Angi finanskladdemalen som avregnede betalinger overføres til.|  
    |**Returkladd navn**|Angi finanskladden som avregnede betalinger overføres til.|  

5.  I hurtigfanen **Innland** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Mottaker ref. 1 - fak.**|Angi teksten som skal skrives ut på betalingsfakturaen.|  
    |**Mottaker ref. 1 - kred.**|Angi teksten som skal skrives ut på betalingsfakturaen ved fradrag av en kreditnota.|  

6.  I hurtigfanen **Utland** fyller du ut feltene som beskrevet i tabellen nedenfor.  

    Denne informasjonen blir bare benyttet hvis kontoen brukes til betalinger utland. Ikke bruk denne hurtigfanene ved remittering til BBS.  

    |Felt|Description|  
    |---------------------------------|---------------------------------------|  
    |**Valutakode**|Angi valutaen som benyttes for bankkontoen.<br /><br /> Hvis kontoen er en valutakonto, må valutakoden angis.|  
    |**Mottakerref. utland**|Angi maltekst som vises på leverandørkortet. Feltet er bare for betalinger utland.|  
    |**Terminskontraktnr.**|Angi nummeret for terminskontrakten hvis transaksjonen er knyttet til en terminskontrakt.|  
    |**Terminskontraktkurs**|Angi valutakursen for terminskontrakten.|  

7.  Velg **OK**.  

## <a name="see-also"></a>Se også  
 [Elektroniske betalinger til leverandører i Norge](electronic-payments-to-vendors-in-norway.md)   
 [Sette opp remitteringsavtaler](how-to-set-up-remittance-agreements.md)   
 [Angi leverandører for remittering](how-to-set-up-vendors-for-remittance.md)   
 [Mottakerreferansekoder](recipient-reference-codes.md)   
 [Opprette remitteringsforslag](how-to-create-remittance-suggestions.md)   
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

