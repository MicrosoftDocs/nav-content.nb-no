---
title: Velg metoden for elektroniske betalinger
description: "Behandle betalinger til leverandører i -vinduet ved å eksportere en fil sammen med betalingsinformasjonen fra kladdelinjene."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: baafa833fb170fb05f866aac91a05085545aaf97
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Betale med tjenesten for bankdatakonvertering eller SEPA-kredittoverføring
Nå kan du behandle betalinger til leverandører i vinduet **Betalingskladd** ved å eksportere en fil sammen med betalingsinformasjonen fra kladdelinjene. Du kan deretter laste opp filen til nettbanken der de relaterte pengeoverføringene behandles. [!INCLUDE[d365fin](includes/d365fin_md.md)] støtter formatet for SEPA-kreidttoverføring, men andre formater for elektroniske betalinger kan være tilgjengelige i ditt land/region.   

 Hvis du vil gjøre det mulig å foreta SEPA-kredittoverføringer, må du først opprette en bankkonto, en leverandør og finanskladden som utbetalingskladden er basert på. Deretter gjør du klar betalinger til leverandører ved å fylle ut vinduet **Betalingskladd** med forfalte betalinger som har angitte bokføringsdatoer.  

> [!NOTE]  
>  Når du har bekreftet at betalingene er behandlet av banken, kan du begynne å bokføre utbetalingskladdelinjene.  

 Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.   

|**Hvis du vil**|**Se**|  
|------------|-------------|  
|Aktiverer tjenesten for bankdatakonvertering for å konvertere en kontoutdragsfil til et format du kan importere, eller konvertere den eksporterte betalingsfilen til formatet som banken krever.|[Konfigurere tjeneste for konvertering av bankdata](bank-how-setup-bank-data-conversion-service.md)|  
|Definere en bankkonto, leverandør og en utbetalingskladd for SEPA-kredittoverføring.|[Definere SEPA-kredittoverføring](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Fylle ut utbetalingskladden med linjer for utestående leverandørfordringer, med mulighet til å sette inn bokføringsdatoer basert på forfallsdatoen til de relaterte kjøpsdokumentene.|[Administrere skyldige beløp](payables-manage-payables.md)|  
|Eksportere utbetalingskladdelinjer til en fil i SEPA-kredittoverføringsformatet.|[Fremgangsmåte: Eksportere betalinger til en bankfil](payables-how-export-payments-bank-file.md)|  
|Gå gjennom hvilke betalinger som er eksportert til hvilke filer.|Kredittoverføringsregistre|  
|Bokfør betalingene når den elektroniske betalingen er behandlet av banken.|[Arbeide med finanskladder](ui-work-general-journals.md)|  

## <a name="see-also"></a>Se også  
[Konfigurere tjeneste for konvertering av bankdata](bank-how-setup-bank-data-conversion-service.md)  
[Definere SEPA-kredittoverføring](finance-how-to-set-up-sepa-credit-transfer.md)  
[Administrere skyldige beløp](payables-manage-payables.md)   
[Arbeide med finanskladder](ui-work-general-journals.md)  
[Innkreve betalinger med SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md)   

