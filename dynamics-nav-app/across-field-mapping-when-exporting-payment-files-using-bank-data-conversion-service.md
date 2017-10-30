---
title: Felttilordning for eksport av bankbetalingsfiler
description: "Når du eksporterer betalingsfiler ved hjelp av konverteringstjenesten for bankdata, blir dataene du eksporterer, eksponert for leverandøren av konverteringstjenesten for bankdata."
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 7eebca3303e9844e4ec8be2940104f9cb7216f6a
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="field-mapping-when-exporting-payment-files-using-bank-data-conversion-service"></a>Felttilordning ved eksport av betalingsfiler ved hjelp av konverteringstjeneste for bankdata
Når du eksporterer betalingsfiler ved hjelp av konverteringstjenesten for bankdata, blir dataene du eksporterer, eksponert for leverandøren av konverteringstjenesten for bankdata. Tjenesteleverandøren er ansvarlig for personvernet vedrørende disse dataene. Hvis du vil ha mer informasjon om hvordan konverteringstjenesten for bankdata fungerer, kan du se [Rammeverket for datautveksling](across-about-the-data-exchange-framework.md).  

> [!CAUTION]  
>  Når du eksporterer betalingsfiler ved hjelp av konverteringstjenesten for bankdata, blir noen av forretningsdataene dine eksponert for leverandøren av tjenesten. Tjenesteleverandøren, AMC Consult A/S, er ansvarlig for personvernet vedrørende disse dataene. Hvis du vil ha mer informasjon, kan du se [personvernpolicyen for AMC](http://go.microsoft.com/fwlink/?LinkId=510158).  

Følgende tabell viser fra hvilke felt i [!INCLUDE[d365fin](includes/d365fin_md.md)] data kan eksporteres til tjenesteleverandøren.  

|Tilordnet felt|Felt i tabell|Bord|Description|  
|------------------|--------------------|-----------|---------------------------------------|  
|Kreditornr.|Kreditornr.|Bankkonto|Identifikatoren som er tilordnet til selskapet av banken for å innkreve betalinger|  
|Bankkontonummer for avsender|Bankkontonr./IBAN|Bankkonto|Bankkontonummeret (IBAN eller annet) til selskapet ditt som er angitt på bankkortet|  
|Klareringsstandard for avsenderbank|Bankklareringsstandard|Bankkonto|Journalen for navn på nasjonale banker som brukes for avsenderbankkontoen|  
|Klareringskode for avsenderbank|Bankklareringskode|Bankkonto|IDen til avsenderens bank i forbindelse med banknavnjournalen som brukes|  
|BIC-kode for avsender|SWIFT-kode|Bankkonto|SWIFT-koden for avsenderbankkontoen|  
|Kontovaluta for avsenderbank|Valutakode|Bankkonto|Valutakoden for avsenderbankkontoen|  
|Bilagsnr.|Bilagsnr.|Finanskladdelinje|Bilagsnummeret på betalingslinjen|  
|Ekst. utligningsdok.nr.|Ekst. utligningsdok.nr.|Finanskladdelinje|Det eksterne bilagsnummeret på fakturaen eller kreditnotaen som betalingslinjen utlignes mot|  
|Mottaker-ID|Kontonummer.|Finanskladdelinje|Kunde- eller leverandørnummeret som er angitt på betalingslinjen|  
|Betalingstype|Betalingstype for bankdatakonvertering|Betalingsmåte|Bankoverføringstypen, for eksempel innenlandsk eller internasjonal|  
|Betalingsreferanse|Betalingsreferanse|Finanskladdelinje|Betalingsreferansen på betalingslinjen|  
|Mottakeradresse|Adresse|Kunde/Leverandør|Mottakeradressen som er angitt på kunde- eller leverandørkortet|  
|Mottakersted|Sted|Kunde/Leverandør|Mottakerpoststedet som er angitt på kunde- eller leverandørkortet|  
|Mottakernavn|Navn|Kunde/Leverandør|Mottakernavnet som er angitt på kunde- eller leverandørkortet|  
|Mottakerens lands-/regionkode|Lands-/regionkode|Kunde/Leverandør|Lands-/regionkode for mottaker som er angitt på kunde- eller leverandørkortet|  
|Mottakerens postnummer|Postnr.|Kunde/Leverandør|Postnummer for mottaker som er angitt på kunde- eller leverandørkortet|  
|Bankkontonummer for mottaker|Bankkontonr./IBAN|Kundens bankkonto / Leverandørs bankkonto|Nummeret (IBAN eller annet) på mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|  
|Klareringskode for mottakerbank|Bankklareringsstandard|Kundens bankkonto / Leverandørs bankkonto|Journalen for navn på nasjonale banker som brukes for mottakerbankkontoen|  
|Klareringsstandard for mottakerbank|Bankklareringskode|Kundens bankkonto / Leverandørs bankkonto|IDen til mottakerbankkontoen i forbindelse med banknavnjournalen som brukes|  
|E-postadresse for mottaker|E-post|Kunde/Leverandør|E-postadressen til mottakeren|  
|Melding til mottaker 1|Melding til mottaker|Finanskladdelinje|Meldingen til mottakeren som er angitt på betalingslinjen|  
|Beløp|Beløp|Finanskladdelinje|Beløpet på betalingslinjen|  
|Valutakode|Valutakode|Finanskladdelinje|Valutakoden på betalingslinjen|  
|Overføringsdato|Bokføringsdato|Finanskladdelinje|Bokføringsdatoen for betalingslinjen|  
|Fakturabeløp|Opprinnelig beløp|Kunde-/Leverandørpost|Beløpet i posten som betalingen utlignes mot|  
|Fakturadato|Bilagsdato|Kunde-/Leverandørpost|Fakturadatoen i posten som betalingen utlignes mot|  
|Mottakerbankadresse|Adresse|Kundens bankkonto / Leverandørs bankkonto|Adressen til mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|  
|Adressen til mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|Sted|Kundens bankkonto / Leverandørs bankkonto|Poststedet til mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|  
|Mottakerbanknavn|Navn|Kundens bankkonto / Leverandørs bankkonto|Navnet på mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|  
|Land/region for mottakerbank|Lands-/regionkode|Kundens bankkonto / Leverandørs bankkonto|Landet/regionen til mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|  
|Mottakerbankens postnummer|Postnr.|Kundens bankkonto / Leverandørs bankkonto|Postnummeret til mottakerbankkontoen som er angitt på kunde- eller leverandørbankkortet|  
|Adresse til avsenderbank|Adresse|Bankkonto|Adressen til avsenderbankkontoen som er angitt på bankkortet|  
|Sted for avsenderbank|Sted|Bankkonto|Poststedet til avsenderbankkontoen som er angitt på bankkortet|  
|Navn for avsenderbank|Navn|Bankkonto|Navnet på avsenderbankkontoen som er angitt på bankkortet|  
|Land/region for avsenderbank|Lands-/regionkode|Bankkonto|Landet/regionen til avsenderbankkontoen som er angitt på bankkortet|  
|Postnummer for avsenderbank|Postnr.|Bankkonto|Postnummeret til avsenderbankkontoen som er angitt på bankkortet|  
|Finanskladdemal|Kladdemalnavn|Finanskladdelinje|Finanskladdemalen som brukes for betalingslinjen|  
|Finanskladdenavn|Kladdenavn|Finanskladdelinje|Finanskladdenavnet som brukes for betalingslinjen|  
|Navn på avsenderbank – datakonvertering|Banknavn – datakonvertering|Bankkonto|Navnet på avsenderbankkontoen som er forespurt av konverteringstjenesten for bankdata og angitt på bankkortet|  

## <a name="see-also"></a>Se også  
[Definere datautveksling](across-set-up-data-exchange.md)  
[Utveksle data elektronisk](across-data-exchange.md)
[Konfigurere konverteringstjenesten for bankdata](bank-how-setup-bank-data-conversion-service.md)   
[Betale med tjenesten for bankdatakonvertering eller SEPA-kredittoverføring](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)   

