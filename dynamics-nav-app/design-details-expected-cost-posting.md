---
title: "Designdetaljer - Bokføre forventet kost"
description: "Forventede kostnader representerer for eksempel overslaget for kjøpspris for en vare du registrerer, før du faktisk mottar fakturaen for varen."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0b14943e1bb214c26dfbae765a2467df1d06e50b
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-expected-cost-posting"></a>Designdetaljer: Bokføre forventet kost
Forventede kostnader representerer for eksempel overslaget for kjøpspris for en vare du registrerer, før du faktisk mottar fakturaen for varen.  

 Du kan bokføre forventet kost på lager og i finans. Når du bokfører et antall som bare er mottatt eller levert, men ikke fakturert, opprettes deretter en verdipost den forventede kostnaden. Denne forventede kostnaden påvirker lagerverdien, men bokføres ikke i finans med mindre du konfigurerer systemet slik at dette gjøres.  

> [!NOTE]  
>  Forventede kostnader behandles bare for varetransaksjoner. Forventede kostnader er ikke for immaterielle transaksjonstyper, for eksempel kapasitet og varegebyr.  

 Hvis bare antallsdelen av en lagerøkning er bokført, vil ikke lagerverdien i Finans endres med mindre du har merket av for **Bokf. av forventet kost i Finans** i vinduet **Lageroppsett**. I slike tilfeller bokføres forventet kost på midlertidige konti på mottakstidspunktet. Når mottaket er ferdigfakturert, balanseres de midlertidige kontiene, og de faktiske kostnadene bokføres til lagerkontoen.  

 For å støtte avstemming og sporing viser den fakturerte verdiposten det forventede kostbeløpet som er bokført på motkonti og midlertidige konti.  

## <a name="example"></a>Eksempel  
 Følgende eksempel viser forventede kostnader hvis det er merket av for **Automatisk kostbokføring** og **Bokf. av forventet kost i Finans** er valgt i vinduet **Lageroppsett**.  

 Du bokfører en bestilling som mottatt. Forventet kostnad er NOK 95,00.  

 **Verdiposter**  

|Bokføringsdato|Posttype|Kostbeløp (forventet)|Forventet kost bokført i Finans|Forventet kostnad|Varepostnr.|Løpenr.|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|01.01.20|Kjøpspris/prod.kost|95,00|95,00|Ja|1|1|  

 **Relasjonsposter i tabellen Finans – varepostrelasjon**  

|Finansløpenr.|Verdiløpenummer|Finansjournalnr.|  
|--------------------|---------------------|-----------------------|  
|1|1|1|  
|2|1|1|  

 **Finansposter**  

|Bokføringsdato|Finanskonto|Kontonummer (En-US-demo)|Beløp|Løpenr.|  
|------------------|------------------|---------------------------------|------------|---------------|  
|01.01.20|Forventet lagerjusteringskonto (midlertidig)|5530|-95,00|2|  
|01.01.20|Lagerkonto (midlertidig)|2131|95,00|1|  

 Senere bokfører du bestillingen som fakturert. Fakturert kost er NOK 100,00.  

 **Verdiposter**  

|Bokføringsdato|Kostbeløp (faktisk)|Kostbeløp (forventet)|Bokført kost|Forventet kostnad|Varepostnr.|Løpenr.|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|15.01.20|100,00|-95,00|100,00|Nei|1|2|  

 **Relasjonsposter i tabellen Finans – varepostrelasjon**  

|Finansløpenr.|Verdiløpenummer|Finansjournalnr.|  
|--------------------|---------------------|-----------------------|  
|3|2|2|  
|4|2|2|  
|5|2|2|  
|6|2|2|  

 **Finansposter**  

|Bokføringsdato|Finanskonto|Kontonummer (En-US-demo)|Beløp|Løpenr.|  
|------------------|------------------|---------------------------------|------------|---------------|  
|15.01.20|Forventet lagerjusteringskonto (midlertidig)|5530|95,00|4|  
|15.01.20|Lagerkonto (midlertidig)|2131|-95,00|3|  
|15.01.20|Konto utl. kj.pris/prod.kost|7291|-100|6|  
|15.01.20|Lagerkonto|2130|100|5|  

## <a name="see-also"></a>Se også
 [Designdetaljer: Kostberegning for beholdning](design-details-inventory-costing.md)   
 [Designdetaljer: Kostjustering](design-details-cost-adjustment.md)   
 [Designdetaljer: Avstemming med konti i Finans](design-details-reconciliation-with-the-general-ledger.md)   
 [Designdetaljer: Lagerbokføring](design-details-inventory-posting.md)   
 [Designdetaljer: Avvik](design-details-variance.md)  
 [Administrere lagerkostnader](finance-manage-inventory-costs.md)  
 [Finans](finance.md)  
 [Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

