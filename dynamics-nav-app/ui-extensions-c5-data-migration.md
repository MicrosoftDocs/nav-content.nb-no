---
title: Bruke utvidelsen C5 Datamigrering
description: "Bruk denne utvidelsen til å overføre kunder, leverandører, varer og finanskonti fra Microsoft Dynamics C5 2012 til Dynamics NAV."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 09/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2307849566a44bb49a5db6965ec3056b1a39684b
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---

# <a name="the-c5-data-migration-extension-for-dynamics-nav"></a>Utvidelsen C5 datamigrering for Dynamics NAV
Denne utvidelsen gjør det enkelt å overføre kunder, leverandører, varer og konti fra Microsoft Dynamics C5 2012 til [!INCLUDE[d365fin](includes/d365fin_md.md)]. 

> [!Note] 
> Selskapet i [!INCLUDE[d365fin](includes/d365fin_md.md)]kan ikke inneholde data. I tillegg, når du starter en migrering, bør du ikke opprette kunder, leverandører, varer eller kontoer til migreringen er ferdig.

## <a name="to-migrate-data"></a>Migrere data
Det tar kun noen få trinn å eksportere data fra C5 og importere dataen inn i [!INCLUDE[d365fin](includes/d365fin_md.md)]: 

1. I C5 bruker du **Eksportere databasen**-funksjonen for å eksportere dataene. Deretter sender du eksportmappen til en komprimert (pakket) mappe.  
2. I [!INCLUDE[d365fin](includes/d365fin_md.md)] velger du ikonet ![Søk etter side eller rapport](media/ui-search/search_small.png "Søk etter side eller rapport"), så velger du **Datamigrering**, og så  **Datamigrering**.
3. Fullfør trinnene i den assisterte oppsettsveiledningen. Pass på at du velger **Importer fra Microsoft Dynamcis C5 2012** som datakilde.  

> [!Note] 
> Firmaer legger ofte til felt for å tilpasse C5 til deres bestemte bransjer. [!INCLUDE[d365fin](includes/d365fin_md.md)] flytter ikke data fra egendefinerte felt. Migreringen mislykkes også hvis du har flere enn 10 egendefinerte felt. 

## <a name="viewing-the-status-of-the-migration"></a>Se statusen for migreringen
Bruk siden **Oversikt over datamigrering** for å overvåke migreringen. Siden viser informasjon om hvor mange enheter som er inkludert i migreringen, status til migreringen, antall varer som er migrert, og om migreringen var vellykket. Den viser også antall feil, gir deg mulighet til å undersøke hva som gikk feil, og gjør det enkelt å gå til enheten for å løse problemene. Hvis du vil ha mer informasjon, kan du se neste avsnitt i dette emnet. 

> [!Note] 
> Mens du venter på resultatet av overføringen, må du oppdatere siden for å vise resultatet.

## <a name="correcting-errors"></a>Feilkorrigering
Hvis det oppstår en feil, viser **Status**-feltet **Fullført med feil**, og **Feilantall** viser hvor mange feil som oppsto. For å se en oversikt over feilene, kan du åpne siden **Datamigreringsfeil** ved å velge:

* Tallet i feltet **Feilantall** for enheten. 
* Enheten og velg deretter handlingen **Vis feil**. 

For å korrigere en feil kan du velge en feilmelding på siden **Datamigreringsfeil**, og deretter velge **Rediger post** for å åpne en side som inneholder den migrerte dataen til enheten. Etter at du har korrigert én eller flere feil, kan du velge **Migrer** for å migrere enheten du har korrigert, uten å starte hele migrerringen på nytt.  

> [!Tip]
> Hvis du har korrigert én eller flere feil, kan du bruke funksjonen **Velg mer** for å velge flere linjer til som skal migreres. Hvis det finnes feil som ikke er viktige å korrigere, kan du velge dem og så velge **Hopp over valg**.

> [!Note]
> Hvis du har varer som er inkludert i en stykkliste, må du kanskje migrere mer enn én gang hvis den opprinnelige varen ikke er opprettet før variantene som refererer til den. Hvis en varevariant opprettes først, kan referansen til den opprinnelige varen føre til en feilmelding.  

## <a name="verifying-data-after-migrating"></a>Kontrollere dataene etter migrering 
Hvis du vil kontrollere at dataene migrert riktig, kan du se på følgende sider i C5 og [!INCLUDE[d365fin](includes/d365fin_md.md)].

|Microsoft Dynamics C5 2012 | [!INCLUDE[d365fin](includes/d365fin_md.md)]|
|-----|-----|
|Kundeposter| Finanskladder|
|Leverandørposter| Finanskladder|
|Vareposter| Varekladder|

I [!INCLUDE[d365fin](includes/d365fin_md.md)]er navnet på kladden for de migrerte dataene **C5MIGRATE**. 

> [!Note]
> Husk at vi migrerer kun åpne poster. Du finner ingen historiske data.

## <a name="stopping-data-migration"></a>Stoppe datamigrering
Du kan stoppe datamigreringen ved å velge **Stopp alle migreringer**. Hvis du gjør dette, blir alle ventende migreringer også stoppet.

## <a name="see-also"></a>Se også
[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)] ved hjelp av utvidelser](ui-extensions.md)  
[Velkommen til [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)  

