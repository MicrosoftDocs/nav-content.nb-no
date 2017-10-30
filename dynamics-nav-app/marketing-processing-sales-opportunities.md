---
title: Behandle salgsmuligheter i salgssykluser
description: Du kan vise, lukke eller slette salgsmuligheter, du kan opprette tilbud og ordrer for salgsmuligheter, og du kan flytte en salgsmulighet gjennom fasene i en salgssyklus.
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9fe0bd97f7493d9acf4ab99a771fd5f6219027f8
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-process-sales-opportunities"></a>Behandle salgsmuligheter
Når du oppretter en salgsmulighet, er det flere funksjoner for å behandle salgsmuligheten og fullføre den.

## <a name="to-view-opportunities"></a>Vise salgsmuligheter
De eksisterende salgsmulighetene er tilgjengelige fra vinduet **Oversikt over salgsmuligheter**. Det finnes ulike metoder for å får tilgang til vinduet for behandling av salgsmuligheter:

| Vise salgsmuligheter for | Deretter |
| --- | --- |
| Alle selgere og kontakter |Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Oversikt over salgsmuligheter**, og velg deretter den relaterte koblingen. |
| En bestemt selger |Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Selgere**, og velg deretter den relaterte koblingen. Velg selger, velg handlingen **Salgsmuligheter** og velg deretter handlingen **Vis**. |
| En bestemt kontakt |Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Kontakter**, og velg deretter den relaterte koblingen. Velg kontakten fra listen, og velg deretter handlingen **Salgsmuligheter**. |

Hver av disse aktivitetene åpner vinduet **Oversikt over salgsmuligheter**.

## <a name="to-close-opportunities"></a>Lukke salgsmuligheter
Du kan lukke salgsmuligheter når forhandlingene er over. Når du lukker en salgsmulighet, kan du oppgi om den ble vunnet eller mistet og årsaken til at du lukker den. Hvis du vil an angi en årsak, må først definere koder for lukkede salgsmuligheter.

1. I vinduet **Oversikt over salgsmuligheter** velger du salgsmuligheten og deretter handlingen **Lukk**. Vinduet **Lukk salgsmulighet** åpnes.
2. Fyll ut de relevante feltene, og klikk deretter **OK**.

   Feltene **Lukk. av salgsmuligh. - kode** og **Lukket den** er obligatoriske og må fylles ut før du velger **Neste**-knappen.

   I feltet **Lukk. av salgsmuligh. - kode** kan du velge fra en av de eksisterende kodene for lukking av salgsmulighet eller legge til en ny kode. Hvis du vil legge til en ny kode fra rullegardinlisten, velger du **Velge fra hele listen** og deretter **ny**. På den nye, tomme linjen fyller du ut feltet **Kode**, **Type** og **Beskrivelse**, og deretter velg du **OK** knappen.

## <a name="to-create-quotes-for-opportunities"></a>Opprette tilbud for salgsmuligheter
Du kan opprette tilbud for kontakter som ikke er registrert som kunder.

1. I vinduet **Oversikt over salgsmuligheter** velger du salgsmuligheten og deretter handlingen **Tilordne nytt tilbud**. Vinduet **Tilbud** åpnes.
2. Fyll ut de aktuelle feltene.

## <a name="to-create-sales-orders-for-opportunities"></a>Opprette ordrer for salgsmuligheter
Du kan opprette ordrer på bakgrunn av tilbudene du har opprettet for salgsmulighetene. Før du kan opprette ordrer for kontaktene, må du opprette kontakten som en kunde. Hvis du vil ha mer informasjon, kan du se [Opprette en kunde, leverandør eller bankkonto fra en kontakt](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).

1. I vinduet **Oversikt over salgsmuligheter** finner du salgsmuligheten du har opprettet et tilbud for.
2. Velg handlingen **Tilordne nytt tilbud**. Vinduet **Tilbud** åpnes, som viser tilbudet du har tilordnet salgsmuligheten.
3. Fyll ut tilleggsfeltene, og klikk deretter handlingen **Lag ordre**.

Når du håndterer salgsmuligheter, kan det være at du må opprette et tilbud for kontakten som salgsmuligheten er knyttet til.

## <a name="to-delete-opportunities"></a>Slette salgsmuligheter
Du kan slette salgsmuligheter etter at du for eksempel har inngått en avtale. Du kan imidlertid bare slette lukkede salgsmuligheter. Det er to metoder for å slette lukkede salgsmuligheter. Du kan slette individuelle lukkede salgsmuligheter fra vinduet **Oversikt over salgsmuligheter**, eller du kan kjøre den satsvise jobben **Slett lukkede salgsmuligheter** for å slette flere salgsmuligheter basert på angitte vilkår.

Hvis du vil slette lukkede salgsmuligheter vinduet **Oversikt over salgsmuligheter**, velger du salgsmuligheten og deretter handlingen **Slett**.

Hvis du vil slette lukkede salgsmuligheter ved hjelp av den satsvise jobben **Slett lukkede salgsmuligheter**, følger du denne fremgangsmåten:

1. Velg ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), angi **Slett salgsmuligheter**, og velg deretter den relaterte koblingen.
2. I inndelingen **Salgsmulighet** definerer du filtrene som angir de lukkede salgsmulighetene du vil slette.
3. Velg **OK**.

Når du har slettet en salgsmulighet, fjernes det fra vinduet **Oversikt over salgsmuligheter**.

## <a name="to-move-an-opportunity-through-sales-cycle-stages"></a>Flytte en salgsmulighet gjennom salgssyklusfaser
Hvis en salgsmulighet følger en salgssyklus, kan du flytte den fremover eller bakover gjennom de ulike fasene, for eksempel flytte til neste eller forrige fase, og til og med hopper over en fase.

1. I vinduet **Oversikt over salgsmuligheter** velger du handlingen **Oppdater**. **Oppdater salgsmulighet** åpnes.
2. Bruk feltet **Handlingstype** for å flytte salgsmuligheten gjennom faser i salgssyklusen:
   * **Neste** flytter salgsmuligheten fremover en fase.
   * **Hopp over** flytter salgsmuligheten fremover én eller flere faser i salgssyklusen, som du angir i feltet **Presentasjon**. Du kan bare hoppe over faser som er satt opp slik at de tillater utelatelse.
   * **Forrige** flytter salgsmuligheten bakover en fase.
   * **Hopp** flytter salgsmuligheten bakover én eller flere faser i salgssyklusen, som du angir i feltet **Presentasjon**.
   * **Oppdater** lar deg endre informasjonen (for eksempel endre evalueringen av salgsutsikter og anslåtte verdier) uten å flytte til en annen fase.
3. Fyll ut de andre feltene etter behov, og klikk deretter **OK**.

## <a name="see-also"></a>Se også
[Salg](sales-manage-sales.md)  
[Opprette og administrere kontakter](marketing-contacts.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

