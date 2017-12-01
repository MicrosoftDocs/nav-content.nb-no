---
title: Utveksle data
description: "Du kan utveksle data mellom [!INCLUDE[d365fin](includes/d365fin_md.md)] og eksterne filer eller strømmer i forbindelse med vanlige forretningsoppgaver, for eksempel sending og mottak av elektroniske dokumenter og import og eksport av bankfiler."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/18/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: d83e68f31edf2dee9e3e5bc5b73a4861cfe919d7
ms.contentlocale: nb-no
ms.lasthandoff: 10/23/2017

---
# <a name="exchanging-data"></a>Utveksle data
Du kan utveksle data mellom [!INCLUDE[d365fin](includes/d365fin_md.md)] og eksterne filer eller strømmer i forbindelse med vanlige forretningsoppgaver, for eksempel sending og mottak av elektroniske dokumenter og import og eksport av bankfiler.  

Før du kan sende og motta elektroniske dokumenter eller importere og eksportere bankfiler, må du definere rammeverket for datautveksling til å behandle datafiler eller -strømmer som er involvert. Du må i tillegg konfigurere relaterte områder. Disse omfatter hoveddata for kunder du sender elektroniske fakturaer til, og konverteringstjenesten for bankdata i tilfelle du distribuerer bankfilkonverteringer til en ekstern tjenesteleverandør. Hvis du vil ha mer informasjon, kan du se [Definere datautveksling](across-set-up-data-exchange.md).  

 Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.  

|**Hvis du vil**|**Se**|  
|------------|-------------|  
|Konvertere salgsdokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)] til et standardisert format og sende dem som elektroniske dokumenter som kundene kan motta til systemet.|[Sende elektroniske dokumenter](sales-how-to-send-electronic-documents.md)|  
|Send PDF-eller bildefiler til en leverandør av OCR-tjenester, og få dem tilbake som elektroniske dokumenter som kan konverteres til dokumentposter i [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Bruke OCR til å konvertere PDF- og bildefiler til elektroniske dokumenter](across-how-use-ocr-pdf-images-files.md)|  
|Motta elektroniske dokumenter, enten fra OCR-tjenesten eller dokumentutvekslingstjenesten, i et standardisert format som du konverterer til de relevante dokumentpostene i [!INCLUDE[d365fin](includes/d365fin_md.md)].|[Motta og konvertere elektroniske dokumenter](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|Importer en bankkontoutdragsfil i vinduet **Betalingsavstemmingskladd** som det første trinnet i avstemming av betalinger eller i vinduet **Bankkontoavstemming** som det første trinnet i avstemming av bankkontoer.|[Utligne betalinger automatisk og avstemme bankkonti](receivables-apply-payments-auto-reconcile-bank-accounts.md)|  
|Eksporter betalinger fra vinduet **Betalingskladd** til en bankfil du laster opp til nettbankkontoen for å få den behandlet.|[Fremgangsmåte: Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md)|  
|Instruere banken om å overføre betalingsbeløpet fra kundenes bankkonti til firmaets konto i henhold til oppsettet av SEPA direct debit.|[Opprette poster for SEPA Direct Debit-oppkreving og eksportere til en bankfil](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md)|  
|Bruk en tjenesteleverandør for valutakurser for å oppdatere **Valutaer**-vinduet.|[Oppdatere valutakurser](finance-how-update-currencies.md)|  
|Vis hvilke filelementer som er tilordnet til felt i [!INCLUDE[d365fin](includes/d365fin_md.md)], når du importerer SEPA CAMT-bankkontoutdragsfiler.|[Felttilordning ved import av SEPA CAMT-filer](across-field-mapping-when-importing-sepa-camt-files.md)|  
|Vis hvilke felt i [!INCLUDE[d365fin](includes/d365fin_md.md)] som er tilordnet til filelementene, når du eksporterer betalingsfiler ved hjelp av konverteringstjenesten for bankdata.|[Felttilordning ved eksport av betalingsfiler ved hjelp av konverteringstjeneste for bankdata](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a>Se også  
[Definere datautveksling](across-set-up-data-exchange.md)  
[Utveksle data elektronisk](across-data-exchange.md)  
[Fakturere salg](sales-how-invoice-sales.md)   
[Registrere kjøp](purchasing-how-record-purchases.md)  
[Inngående dokumenter](across-income-documents.md)  
[Generelle forretningsfunksjoner](ui-across-business-areas.md)  

