---
title: "Behandle inngående og utgående KI-transaksjoner"
description: "Konserninterne transaksjoner du mottar fra de konserninterne partnerne dine, er oppført i den konserninterne innboksen der du behandler dem manuelt eller automatisk."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoming document
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 869dacac09019fda487e8ac18a5c8ff5d0fd17ac
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-the-intercompany-inbox-and-outbox"></a>Administrere den konserninterne innboksen og utboksen
Alle de konserninterne transaksjonene du mottar elektronisk fra de konserninterne partnerne, er oppført i den konserninterne innboksen.  

## <a name="organizing-the-inbox"></a>Ordre innboksen  
 Du kan bruke filterfeltene øverst i innboksvinduet til å bestemme hvilke transaksjoner som skal vises i vinduet. Hvis du for eksempel bare vil se på transaksjoner som en bestemt partner har opprettet, kan du angi filtre i filtrene for **transaksjonskilde** og **kode for konsernintern partner**.  

### <a name="transaction-source"></a>Transaksjonskilde  
Hva du kan gjøre med en transaksjon, avhenger av om den ble:  

- Opprettet av den konserninterne partneren  
- Avvist av den konserninterne partneren og returnert til deg  

Du kan bruke feltet **Vis transaksjonskilde** til å filtrere vinduet **Konserninterne inngående transaksjoner** slik at det bare viser én av disse transaksjonstypene. (Du kan også filtrere etter konsernintern partner eller etter innholdet i **Linjehandling**-feltet.)  

#### <a name="created-by-intercompany-partner"></a>Opprettet av konsernintern partner  
 Når du mottar en ny transaksjon som ble opprettet av partneren, kan du velge å:

- Godta transaksjonen  
- Avvise transaksjonen (returnere den til partneren)  
- Avbryte transaksjonen (slette transaksjonen, men ikke returnere den til partneren)  

#### <a name="returned-from-intercompany-partner"></a>Returnert fra konsernintern partner  
 Hvis transaksjonen ble avvist av den konserninterne partneren, kan du bare avbryte transaksjonen i innboksen. Deretter må du opprette korrigeringslinjer eller reversere kladden eller bilaget i selskapet.  

## <a name="re-creating-inbox-entries"></a>Opprette innboksposter på nytt  
 Hvis du godtok en transaksjon i innboksen, men deretter slettet bilaget eller kladden i stedet for å bokføre det/den, kan du opprette innboksposten på nytt og godta den på nytt.  

## <a name="getting-an-overview-of-intercompany-transactions-for-a-period"></a>Få oversikt over konserninterne transaksjoner for en periode  
 Du kan få oversikt over alle de konserninterne transaksjonene du har sendt og mottatt i en periode. Rapporten **Konserninterne transaksjoner** viser alle konserninterne finansposter, kundeposter og leverandørposter.

 > [!NOTE]  
 > Hvis de konserninterne partnerne er i samme database, overføres transaksjoner uten å måtte filen eller e-post. Se feltet **Overføringstype** i vinduet **Konsernintern partner**. <br /><br />
I så fall kan du konfigurere systemet til å hoppe over innboksen og utboksen ved å merke av for henholdsvis **Godta transaksjoner automatisk** i vinduet **Konsernintern partner** og **Send transaksjoner automatisk** i vinduet **Konserninternt oppsett**.

## <a name="to-import-intercompany-transactions-from-a-file"></a>Slik importerer du konserninterne transaksjoner fra en fil  
Hvis du har en konsernintern partner som ikke er i samme database som selskapet ditt, kan du motta konserninterne transaksjoner fra partneren i en XML-fil. Deretter må du importere transaksjonene til innboksen.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Selskapsopplysninger**, og velg deretter den relaterte koblingen.
2. Lagre filen på lokasjonen du har angitt i feltet **Detaljer om konsernintern innboks** i vinduet **Selskapsopplysninger**.  
3. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Konserninterne inngående transaksjoner**, og velg deretter den relaterte koblingen.
4. I vinduet **Konserninterne inngående transaksjoner** velger du **Importer transaksjonsfil**.  
5. I vinduet som vises, velger du XML-filen som inneholder transaksjonene, og deretter velger du **Åpne**-knappen.  

Transaksjonene importeres til innboksen, og du kan nå behandle dem.

## <a name="to-process-incoming-intercompany-transactions"></a>Slik behandler du inngående konserninterne transaksjoner  
Når de konserninterne partnerne sender deg konserninterne transaksjoner, ender transaksjonene opp i den konserninterne innboksen. Du må vurdere hver transaksjon i innboksen og utføre de nødvendige handlingene.  

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Konserninterne inngående transaksjoner**, og velg deretter den relaterte koblingen.  
2. I vinduet **Konserninterne inngående transaksjoner** velger du en linje og velger en handling som **Godta**, for å behandle linjen.
3. I vinduet **Fullfør KI-innbokshandling** fyller du ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Velg **OK**.  

For linjer som du behandlet med **Godta**-handlingen, bilag eller kladdelinjer vil bli opprettet i selskapet. Åpne hvert bilag eller hver kladd, gjør de nødvendige endringene, og bokfør dem.  

Linjene som du behandlet med **Gå tilbake til partner**-handlingen, vil bli flyttet til utboksen fra der du kan deretter sende dem til partneren.

For linjer du behandlet med **Returnert av partner**-handlingen, må du nå bokføre en korreksjon av den opprinnelige transaksjonen du bokførte i selskapet ditt.

## <a name="to-process-outgoing-intercompany-transactions"></a>Slik behandler du utgående konserninterne transaksjoner  
Når du bokfører konserninterne kladder eller bilag eller sender en konsernintern bestillingsbekreftelse, sendes transaksjonene til den konserninterne utboksen. Du må åpne utboksen og behandle dem for at de skal bli sendt videre til de konserninterne partnerne.  

1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Konserninterne utgående transaksjoner**, og velg deretter den relaterte koblingen.  
2. I vinduet **Konserninterne utgående transaksjoner** velger du en linje og velger en handling som **Gå tilbake til innboks**, for å behandle linjen.

Linjene som du behandlet med **Send til konsernintern partner**-handlingen, vil bli sendt til innboksen til den relevante partneren.

Linjene som du behandlet med **Gå tilbake til innboks**-handlingen, vil bli flyttet til innboksen der du kan godta dem til å opprette bilag eller kladdelinjer i selskapet.  

For linjer du behandlet med **Avbryt**-handlingen, må du nå bokføre en korreksjon av den opprinnelige transaksjonen du bokførte i selskapet ditt.  

## <a name="to-recreate-intercompany-inbox-transactions"></a>Slik oppretter du konserninterne innbokstransaksjoner på nytt:  
Noen ganger vil du kanskje opprette en transaksjon på nytt i innboksen eller utboksen. Hvis du for eksempel godtok en transaksjon i innboksen, men deretter slettet bilaget eller kladden i stedet for å bokføre det/den, kan du opprette innboksposten på nytt og godta den på nytt.  

Følgende fremgangsmåte beskriver hvordan du oppretter innbokstransaksjoner på nytt, men de samme trinnene gjelder også for utboksen.

  1.  Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Håndterte inngående KI-transaksjoner**, og velg deretter den relaterte koblingen.  

  2.  I vinduet **Håndterte inngående KI-transaksjoner** velger du linjen med transaksjonen du vil opprette på nytt i innboksen, og velger deretter **Opprett inngående transaksjon på nytt**.  

## <a name="see-also"></a>Se også
[Behandle konserninterne transaksjoner](intercompany-manage.md)  
[Finans](finance.md)  
[Konfigurere finans](finance-setup-finance.md)  
[Arbeide med finanskladder](ui-work-general-journals.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

