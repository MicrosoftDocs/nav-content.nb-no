---
title: Opprette nummerserier
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a>Opprette nummerserier

For hvert selskap som opprettes, må du tilordne unike identifikasjonskoder til elementer som for eksempel hovedbokkontoer, kunde- og leverandørkontoer, fakturaer og dokumenter. Nummerering er ikke bare viktig for identifikasjonsformål. Med et godt utformet nummereringssystem er det enklere å styre og analysere selskapet, og antall feil som forekommer ved dataregistrering reduseres.

Du kan lage et komplett nummereringssystem med et ubegrenset antall nummerserier. Du kan bruke nummerserier for alle typer dokumenter og kladder, så vel som for hoveddata som for eksempel kunder, varer og jobber.

Du kan kombinere bruken av nummerserier med manuell nummerering.

Et nummereringssystem lager du ved å opprette én eller flere koder for hver hoveddatatype eller dokumenttype. Du kan for eksempel opprette én kode for å nummerere kunder, en annen kode for å nummerere salgsfakturaer, og enda en kode for å nummerere dokumenter i finanskladder.

Når du har opprettet en kode, må du opprette minst én nummerserielinje. Nummerserielinjen inneholder informasjon som for eksempel første og siste nummer i serien, samt startdato. Du kan opprettet mer enn én nummerserielinje per nummerseriekode, med ulik startdato for hver linje. Seriene brukes i rekkefølge, og hver serie starter på sin respektive startdato.

Hvis du vil bruke mer enn én nummerseriekode for én type hoveddata - det vil si hvis du for eksempel vil bruke ulike nummerserier for ulike varekategorier - kan du bruke nummerserieforbindelser.

I tillegg til numrene du tilordner manuelt eller ved hjelp av nummereringssystemet, blir det automatisk tilordnet fortløpende nummerering av alle transaksjoner (poster). Disse numrene kan ses i **Løpenr.** -feltet i alle postvinduene. Du kan ikke endre eller slette disse numrene.

## <a name="to-create-relationships-between-number-series"></a>Slik oppretter du forbindelser mellom nummerserier
Hvis du har opprettet mer enn én nummerseriekode for den samme typen grunnleggende opplysninger eller transaksjoner, kan du opprette forbindelser mellom kodene. Denne funksjonen kan hjelpe deg med å velge mellom koder når du bruker et nummer.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Nummerserie** og velger deretter den relaterte koblingen.
2. Velg linjen med nummerserien du vil opprette forbindelser for, og velg deretter **Forbindelser**.
3. I **Seriekode**-feltet angir du koden for nummerserien du vil knytte til serien du valgte i trinn 2.
4. Legg til en linje for hver kode du vil knytte til den valgte nummerserien.
5. Lukk vinduet.

Når du så registrerer noe som trenger et nummer, kan du bruke forbindelsene du har opprettet til å velge mellom nummerseriene som er koblet til hverandre.

## <a name="see-also"></a>Se også
[Arbeide med Dynamics NAV](ui-work-product.md)

