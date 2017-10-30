---
title: Sende elektroniske dokumenter
description: "Lær hvordan du sender fakturaer elektronisk."
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5920ed97f054b3e7882f40f2fceec76183800297
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-send-electronic-documents"></a>Sende elektroniske dokumenter
Den generelle versjonen av [!INCLUDE[d365fin](includes/d365fin_md.md)] kan sende elektroniske fakturaer og kreditnotaer i PEPPOL-format, som støttes av de største leverandørene av dokumentutvekslingstjenester. En leverandør av dokumentutvekslingstjenester fordeler elektroniske dokumenter mellom handelspartnere. Hvis du vil ha støtte for andre elektroniske dokumentformater, kan du bruke rammeverket for datautveksling.  

 I den generelle versjonen av [!INCLUDE[d365fin](includes/d365fin_md.md)] er en dokumentutvekslingstjeneste forhåndskonfigurert og klar til å bli definert for firmaet. Hvis du vil ha mer informasjon, kan du se [Konfigurere en dokumentutvekslingstjeneste](across-how-to-set-up-a-document-exchange-service.md).  

 Hvis du vil sende en salgsfaktura som et elektronisk PEPPOL-dokument, velger du alternativet **Elektronisk dokument** i dialogboksen **Bokfør og send**, der du også kan konfigurere kundens standardprofil for dokumentsending. Først må du definere forskjellige hoveddata, for eksempel firmainformasjon, kunder, varer og enheter. Disse brukes til å identifisere forretningspartnere og elementer ved konvertering av data i feltene [Konfigurere sending og mottak av elektroniske dokumenter](across-how-to-set-up-electronic-document-sending-and-receiving.md).  

### <a name="to-send-an-electronic-sales-invoice"></a>Slik sender du en elektronisk salgsfaktura:  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Salgsfakturaer**, og velg deretter den relaterte koblingen.  

2.  Opprett en ny salgsfaktura.  

3.  Når salgsfakturaen er klar til fakturering, velger du **Bokfør og send** i **Handlinger**-kategorien i **Bokføring**-gruppen.  

     Hvis kundens standard sendingsprofil er **Elektronisk dokument**, vil den vises i dialogboksen **Bokfør og send bekreftelse**, og du trenger bare å velge **Ja**-knappen for å bokføre og sende fakturaen elektronisk i det valgte formatet.  

4.  I dialogboksen **Bokfør og send bekreftelse** velger du AssistEdit-knappen til høyre for feltet **Send dokument til**.  

5.  I dialogboksen **Send dokument til** i feltet **Elektronisk dokument** velger du **Gjennom dokumentutvekslingstjeneste**.  

6.  I **Format**-feltet velger du **PEPPOL**.  

7.  Velg **OK**-knappen. Dialogboksen **Bokfør og send bekreftelse** vises. **Elektronisk dokument (PEPPOL)** legges til i **Send dokument til**-feltet.  

8.  Velg **Ja**-knappen.  

     Salgsfakturaen bokføres og sendes til kunden som et elektronisk dokument i formatet PEPPOL.  

    > [!NOTE]  
    >  Du kan også sende en bokført salgsfaktura som et elektronisk dokument. Fremgangsmåten er den samme som beskrevet i dette emnet for ikke-bokførte salgsdokumenter. I vinduet **Bokført salgsfaktura** i fanen **Handlinger** i gruppen **Generelt**, velger du **Aktivitetslogg** for å vise statusen for det elektroniske dokumentet. Hvis du vil ha mer informasjon, kan du se **Aktivitetslogg**.  

## <a name="see-also"></a>Se også  
[Fakturere salg](sales-how-invoice-sales.md)  
[Definere en profil for dokumentsending](sales-how-setup-document-send-profiles.md)  
[Konfigurere sending og mottak av elektroniske dokumenter](across-how-to-set-up-electronic-document-sending-and-receiving.md)  
[Konfigurere en dokumentutvekslingstjeneste](across-how-to-set-up-a-document-exchange-service.md)  
[Definere datautvekslingsdefinisjoner](across-how-to-set-up-data-exchange-definitions.md)  
[Utveksle data elektronisk](across-data-exchange.md)  
[Generelle forretningsfunksjoner](ui-across-business-areas.md)  

