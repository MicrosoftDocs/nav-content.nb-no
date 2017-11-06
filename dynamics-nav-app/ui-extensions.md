---
title: "Installere utvidelser for � tilpasse Dynamics NAV"
description: "Finn ut hvordan du legger til funksjoner og tilpasser Dynamics NAV ved � installere utvidelser."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: app, add-in, manifest, customize
ms.date: 07/07/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 109eb8d0e2a38566739878ef513ffa3bec8dcd30
ms.contentlocale: nb-no
ms.lasthandoff: 10/26/2017

---
# <a name="customizing-dynamics-nav-using-extensions"></a>Tilpasse Dynamics NAV ved hjelp av utvidelser
Du kan endre [!INCLUDE[d365fin](includes/d365fin_md.md)] ved � installere utvidelser som for eksempel legger til funksjonalitet, endrer virkem�te eller gir deg tilgang til nye elektroniske tjenester.
N�r du starter [!INCLUDE[d365fin](includes/d365fin_md.md)] for f�rste gang, er noen utvidelser allerede installert for deg. Over tid gj�res flere utvidelser tilgjengelig for deg, og du kan deretter velge om du vil bruke utvidelsen eller ikke.

Microsoft tilbyr for eksempel en utvidelse som kan gi integrering med PayPal Payments Standard. Denne utvidelsen er installert som standard.
Hvis en annen utvidelse gj�res tilgjengelig som gir integrasjon med en annen betalingstjenesten, kan du installere den nye utvidelsen og deretter velger hvilke av de to tjenestene du vil bruke.  

Du administrerer utvidelsene i vinduet **Administrasjon av utvidelse**. Du kan g� til dette vinduet fra Hjem. Du kan ogs� velge ikonet **S�k etter side eller en rapport** ![S�k etter side eller rapport](media/ui-search/search_small.png "S�k etter side eller rapport") i �vre h�yre hj�rne, angi **Utvidelse**, og deretter velger du den beslektede koblingen.  

> [!NOTE]  
>   Hvis du mener at du skal ha tilgang til en utvidelse, men ikke finner funksjonaliteten, kontrollerer du vinduet **Administrasjon av utvidelse**. Hvis utvidelsen ikke er oppf�rt der, kan du installere den, som beskrevet i delen nedenfor.  

## <a name="installing-an-extension"></a>Installere en utvidelse
Du kan f� nye utvidelser fra markedsplassen p� [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1). Her kan du se alle tilgjengelige utvidelser for [!INCLUDE[d365fin](includes/d365fin_md.md)], og du kan f� apper, utvidelser og innholdspakker for andre Microsoft-produkter. Definer de aktuelle filtrene, ta en titt p� informasjonen for hver utvidelse, og f� en utvidelse for [!INCLUDE[d365fin](includes/d365fin_md.md)].  
> [!NOTE]  
>   Logg p� [AppSource.microsoft.com](https://appsource.microsoft.com/) ved � bruke e-postkontoen du bruker med [!INCLUDE[d365fin](includes/d365fin_md.md)]. Bruk samme e-postkonto for andre tjenester og produkter for en problemfri opplevelse.  

Du kan ogs� g� til markedsplassen fra [!INCLUDE[d365fin](includes/d365fin_md.md)]. I vinduet **Administrasjon av utvidelse** kan du se utvidelsene som er installert, og du kan �pne **Markedsplass for utvidelser**-siden som viser [!INCLUDE[d365fin](includes/d365fin_md.md)]-utvidelsene som for �yheblikket er tilgjengelige i AppSource. Hvis du velger *Flere apper*-koblingen, kommer du til [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).  

Hvis du velger en utvidelse, kan du lese om hva utvidelsen gj�r, og du kan f� tilgang til hjelp for utvidelsen for � finne ut mer. N�r du skaffer en utvidelse, m� du godta vilk�rene for bruk. Hvis du f�r utvidelsen fra webomr�det for AppSource, logges du p� [!INCLUDE[d365fin](includes/d365fin_md.md)] for � fullf�re installasjonen.  

N�r du installerer en utvidelse, m� du kanskje konfigurere den, for eksempel angi en konto for bruk med utvidelsen **PayPal-betalingsstandard for [!INCLUDE[d365fin](includes/d365fin_md.md)]**.
Andre utvidelser legger for eksempel ganske enkelt til felt p� en eksisterende side, eller de legger til en ny side.   

Hvis du avinstallerer en utvidelse og du deretter ombestemmer deg, kan du installere den p� nytt. N�r du avinstallerer en utvidelse som du har brukt, beholdes dataene, slik at hvis du installerer utvidelsen p� nytt, er dataene fremdeles tilgjengelige.  

Noen utvidelser leveres av Microsoft, og andre utvidelser leveres av [andre selskaper](ui-extensions-other.md). Alle utvidelser testes f�r de blir gjort tilgjengelige for deg, men vi anbefaler at du g�r til de angitte koblingene som f�lger med hver utvidelse, for � finne ut mer om utvidelsen f�r du velger � installere den.  

Microsoft tilbyr f�lgende utvidelser:  

* [Dynamics GP-datamigrering](ui-extensions-dynamicsgp-data-migration.md)  
* [PayPal Payments Standard](ui-extensions-paypal-payments-standard.md)  
* [Datamigrering for QuickBooks](ui-extensions-quickbooks-data-migration.md)  
* [Salgs- og lagerprognose](ui-extensions-sales-forecast.md)  
* [Ceridian l�nn](ui-extensions-ceridian-payroll.md)  
* [Quickbooks Payroll-filimport](ui-extensions-quickbooks-payroll.md)  
* [WorldPay Payments Standard](ui-extensions-worldpay-payments-standard.md)
* [GetAddress.io UK Postcodes](ui-extensions-getaddressio.md)
* [QuickBooks Online Data Migration](ui-extensions-quickbooks-online-data-migration.md)
* [Regnskapsf�rerportal](ui-extensions-accountant-portal.md)  
* [Image Analyzer](ui-extensions-image-analyzer.md)

> [!NOTE]  
>  Nye utvidelser er ikke tilgjengelige i AppSource like etter at vi har kunngjort en oppdatering. Du kan f�lge med p� utvidelsene p� [AppSource.microsoft.com](https://appsource.microsoft.com/en-us/marketplace/apps?product=dynamics-365%3Bdynamics-365-for-financials&page=1).

## <a name="see-also"></a>Se ogs�
[Aktiver kundebetalinger gjennom PayPal](sales-how-enable-payment-service-extensions.md)  
[Overf�re forretningsdata fra andre �konomisystemer](upload-data.md)    
[[!INCLUDE[d365fin](includes/d365fin_md.md)]-utvidelser fra andre leverand�rer](ui-extensions-other.md)  
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  

##


