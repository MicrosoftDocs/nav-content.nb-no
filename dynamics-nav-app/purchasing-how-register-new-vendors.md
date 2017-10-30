---
title: "Opprette et leverandørkort for å registrere en ny leverandør"
description: "Finn ut hvordan du oppretter et leverandørkort for å registrere en ny leverandør."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c7fee8b43940fc5e5fb020b4ca1ac9b27b90decd
ms.contentlocale: nb-no
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-new-vendors"></a>Registrere nye leverandører
Leverandører tilbyr produktene du selger. Hver leverandør du kjøper fra, må være registrert som et leverandørkort.

Før du kan registrere nye leverandører, må du definere forskjellige kjøpskoder som du kan velge fra når du fyller ut leverandørkort. Når du har angitt alle nødvendige hoveddata, kan du konfigurere leverandøren ytterligere, for eksempel angi betalingsprioritet og vise en oversikt over varer som leverandøren og andre leverandører kan levere. En annen gruppe med oppsettsoppgaver for leverandører er å registrere avtaler om rabatter, priser og betalingsmåter. Hvis du vil ha mer informasjon, kan du se [Definere kjøp](purchasing-setup-purchasing.md).

Leverandørkort inneholder informasjon som er nødvendig for å kjøpe produkter fra leverandøren. Hvis du vil ha mer informasjon, kan du se [Registrere kjøp](purchasing-how-record-purchases.md) og [Registrere nye varer](inventory-how-register-new-items.md).

> [!NOTE]  
>   Hvis det finnes leverandørmaler for ulike leverandørtyper, vises et vindu når du oppretter et nytt leverandørkort der du kan velge en passende mal. Hvis det bare finnes én leverandørmal, brukes alltid denne malen i nye leverandørkort.

## <a name="to-create-a-new-vendor-card"></a>Opprette et nytt leverandørkort
1. På Hjem-siden velger du **Leverandører** for å åpne listen over eksisterende leverandører.  
2. I vinduet **Leverandører** velger du **Ny**.

    Hvis det finnes mer enn én leverandørmal, åpnes et vindu der du kan velge en leverandørmal. I det tilfellet følger du de to neste trinnene.
3. I vinduet **Velg en mal for en ny leverandør** velger du malen som du vil bruke for det nye leverandørkortet.
4. Velg **OK**. Det åpnes et nytt leverandørkort med noen felt som er fylt ut med informasjon fra malen.
5. Fortsette med å fylle ut eller endre feltet på leverandørkortet etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Hvis du ikke vet fakturaadressen som skal brukes for hver eneste faktura fra en leverandør, fyller du ikke ut feltet **Betal til-levrd.nr.** på leverandørkortet. I stedet velger du betal til-leverandørnummeret når du har definert en forespørsel, bestilling eller et fakturahode.

Leverandøren er nå registrert, og leverandørkortet er klart til å brukes på kjøpsdokumenter.

Hvis du vil bruke dette leverandørkortet som en mal når du oppretter nye leverandørkort, kan du lagre det som en leverandørmal. Hvis du vil ha mer informasjon, kan du se følgende avsnitt:

## <a name="to-save-the-vendor-card-as-a-template"></a>Lagre leverandørkortet som en mal
1. I vinduet **Leverandørkort** velger du handlingen **Lagre som mal**. **Leverandørmal**  -vinduet åpnes og viser leverandørkortet som en mal.
2. Fyll ut feltene etter behov. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Hvis du vil bruke dimensjoner i maler, velger du handlingen **Dimensjoner**. **Dimensjonsmaler**-vinduet åpnes med alle dimensjonskoder som er definert for leverandøren.
4. Rediger eller angi dimensjonskoder som skal gjelde for nye leverandørkort som opprettes ved hjelp av malen.
5. Når du har fullført den nye leverandørmalen, kan du velge **OK**-knappen.  
   Leverandørmalen legges til i listen over leverandørmaler, slik at du kan bruke den til å opprette nye leverandørkort.

## <a name="see-also"></a>Se også
[Innkjøp](purchasing-manage-purchasing.md)  
[Registrere kjøp](purchasing-how-record-purchases.md)   
[Arbeide med [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

