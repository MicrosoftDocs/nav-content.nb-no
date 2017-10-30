---
title: "EHF – Elektronisk fakturering i Norge"
description: "Selskaper som må sende salgsfakturaer og kreditnotaer elektronisk til norsk offentlig sektor i Elektronisk Handelsformat (EHF) basert på UBL (Universal Business Language)."
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
ms.openlocfilehash: c014c393b43608fdaf2ce5ec2e9c1b7e7f0d8ed9
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="ehf-electronic-invoicing-in-norway"></a>EHF – Elektronisk fakturering i Norge
Selskaper som må sende salgsfakturaer og kreditnotaer elektronisk til norsk offentlig sektor i Elektronisk Handelsformat (EHF) basert på UBL (Universal Business Language). Hvis et selskap ikke sender dokumentene elektronisk, kan myndighetene nekte betaling. Standardformatet som støttes for elektronisk utveksling mellom parter, er formatet Ehandel.no.  

Hvis du vil ha mer informasjon om elektronisk fakturering i EHF, kan du se [Implementeringsveiledning for EHF: Faktura og kreditnota](http://www.nets.eu/no-nb/support/Test%20og%20Implementering/eFaktura%20B2B%20Utsteder/Documents/Imp%20guide%20eng.pdf) og [EHF-faktura](http://www.anskaffelser.no/ehf-formater-innhold/pages-english/ehf-invoice).  

## <a name="implementation-in-includenavnowincludesnavnowmdmd"></a>Implementering i [!INCLUDE[navnow](../../includes/navnow_md.md)]  
 Gjeldende krav for å sende elektroniske fakturaer er basert på standarden Universal Business Language (UBL) versjon 2.1. Hvis du vil ha mer informasjon, kan du se nettstedet til [OASIS UBL](http://go.microsoft.com/fwlink/?LinkId=212593). De genererte XML-dokumentene kan deretter sendes til kunden.  

 Hvis du vil sende dokumenter elektronisk, må du tilordne EAN-lokasjonsnumre (European Article Numbering) og kontokoder til de aktuelle kundene i **Kundekort**-vinduet. Se [Sette opp kunder for EHF](how-to-set-up-customers-for-ehf.md) for mer informasjon. Disse numrene inkluderes når du oppretter dokumenter, og bokfører eller utsteder dem. Nå dokumentene er bokført eller utstedt, kan du opprette elektroniske versjoner som skal sendes til kunden.  

 [!INCLUDE[navnow](../../includes/navnow_md.md)] eksporterer enkelte elektroniske dokumenter i versjon 2.0, som bruker UBL versjon 2.1. Du kan sende følgende typer dokumenter:  

- Salgsfaktura  
- Servicefaktura  
- Salgskreditnota  
- Salgskreditnota (service)  

 [!INCLUDE[navnow](../../includes/navnow_md.md)] eksporterer andre elektroniske dokumenter i versjon 1.6, som bruker UBL versjon 2.0. Du kan sende følgende typer dokumenter:  

- Rentenota  
- Purring  

De elektroniske dokumentene lagres i lokasjonene som defineres i vinduet Salgsoppsett.  

## <a name="vat-treatment"></a>Mva-justering  
 Mva-prosenter og transaksjonstypen bestemmer mva-typen som eksporteres i det elektroniske dokumentet.  

|XML|Type|Prosentsats|  
|---------|----------|---------------------|  
|S|Utgående mva, vanlige sats|25|  
|H|Utgående mva, redusert sats – matvarer og drikkevarer|15|  
|R|Utgående mva, redusert sats – rå fisk|11.11|  
|AA|Utgående mva, lav sats|8|  
|Ø|Mva-fritak|0|  
|Z|Mva-fritak (varer og tjenester som ikke omfattes av mva-bestemmelsene)|Ingen, rapporteres som 0|  
|K|Utslippstillatelser for private og offentlige bedrifter – kjøperen beregner mva|Ingen, rapporteres som 0|  

## <a name="see-also"></a>Se også  
 [Sette opp kunder for EHF](how-to-set-up-customers-for-ehf.md)

