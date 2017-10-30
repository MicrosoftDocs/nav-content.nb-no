---
title: Administrere aktiva
description: "Les om aktivafunksjonaliteten i Dynamics NAV, og få en oversikt over hvordan du arbeider med aktiva."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: machinery, buildings
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: baf87f3059988056d308f906a59f8b5c75a78784
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="fixed-assets"></a>Anleggsmidler
Aktivafunksjonene i [!INCLUDE[d365fin](includes/d365fin_md.md)] gir en oversikt over hvilke aktiva du har, og hjelper deg med å utføre riktig periodisk avskrivning. De hjelper deg dessuten med å styre vedlikeholdskostnadene, håndtere forsikringspoliser, bokføre aktivatransaksjoner og generere forskjellige rapporter og statistikker.

For hvert enkelt aktiva må du definere et kort som inneholder opplysninger om aktivaet. Du kan definere bygninger eller produksjonsutstyr som hovedaktiva i en komponentoversikt, og du kan gruppere dem på forskjellige måter, som etter klasse, avdeling eller lokasjon. Deretter kan du begynne å kjøpe, vedlikeholde og selge aktiva. Du kan også definere budsjetterte aktiva. Dette gjør det mulig å ta med eventuelle forventede anskaffelser og salg i rapporter.

Hvis du vil holde rede på aktivaavskrivninger samt andre finansielle transaksjoner knyttet til aktiva, definerer du ett eller flere avskrivningstablåer for hvert aktiva i firmaet. Avskrivning gjøres ved å kjøre en rapport for å beregne periodiske avskrivninger og fylle ut en kladd med de resulterende postene, klare til å bokføres. [!INCLUDE[d365fin](includes/d365fin_md.md)] støtter flere ulike avskrivningsmetoder. Hvis du vil ha mer informasjon, kan du se [Avskrivningsmetoder](fa-depreciation-methods.md). Du kan definere flere avskrivningstablåer per aktiva for ulike formål, for eksempel ett for mva-rapportering og et annet for intern rapportering.

For hvert enkelt aktiva kan du registrere vedlikeholdskostnader og dato for neste service. Det kan være viktig å holde oversikt over vedlikeholdsutgifter i forbindelse med budsjettering og dessuten når det gjelder avgjørelser om utskiftning av aktiva.

Hvert aktiva kan knyttes til én eller flere forsikringspoliser. Det er dermed lett å kontrollere at beløpene for forsikringspolisen er i overensstemmelse med verdien på aktivaene som er knyttet til polisen. Dette gjør det dessuten enkelt å følge med på de årlige forsikringspremiene.

> [!NOTE]  
>   Du kan registrere aktivatransaksjoner i vinduet **Aktivafinanskladd** eller **Aktivakladd**, avhengig av om transaksjonene er for finansiell rapportering eller intern håndtering. Hjelp for aktiva beskriver bare hvordan du bruker **Aktiva finanskladd**-vinduet. Se [Definere avskriving av aktiva](fa-how-setup-depreciation.md) hvis du vil ha mer informasjon.

Før du kan begynne å behandle aktiva, må du definere standardverdier, aktivaregnskap, bokføringsgrupper, fordelingsnøkler, kladder og bokføringstyper. Hvis du vil ha mer informasjon, kan du se [Definere aktiva](fa-setup.md).

Tabellen nedenfor beskriver en sekvens av oppgaver, og har koblinger til emnene som beskriver dem.

| Hvis du vil | Se |
| --- | --- |
| Opprette aktiva, tilordne avskrivningsmetoder, bokføre anskaffelser, skrapverdier og skrive ut aktivaoversikter. |[Anskaffe aktiva](fa-how-acquire.md) |
| Registrere servicebesøk, bokføre vedlikeholdskostnader og overvåke vedlikeholdskostnader. |[Vedlikeholde aktiva](fa-how-maintain.md) |
| Oppdatere forsikringsopplysninger, bokføre anskaffelseskostnader til forsikringspoliser, endre forsikringsdekningen, vise forsikringsstatistikk og vise forsikringspoliser. |[Forsikre aktiva](fa-how-insure.md) |
| Klassifisere aktiva på nytt, overføre aktiva til ulike lokasjoner, og dele opp eller knytte sammen aktiva. |[Overføre, dele opp eller kombinere aktiva](fa-how-trans-split-combine.md) |
| Justere verdier for aktiva og bokføre oppskrivnings- og nedskrivningstransaksjoner. |[Revaluere aktiva](fa-how-revalue.md) |
| Beregne avskrivning, bokføre avskrivning og analysere avskrivning i aktivarapporter. |[Avskrive eller amortisere aktiva](fa-how-depreciate-amortize.md) |
| Bokføre salgstransaksjoner, vise salgsposter og bokføre delvise salg. |[Avhende eller trekke tilbake aktiva](fa-how-dispose-retire.md) |
| Administrere aktivabudsjetter, og budsjettere anskaffelseskostnader, salg av aktiva og avskrivninger. |[Behandle budsjetter for aktiva](fa-how-manage-budgets.md) |

## <a name="see-also"></a>Se også
[Definere aktiva](fa-setup.md)  
[Tilpasse [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)  
[Finans](finance.md)  
[Velkommen til [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

