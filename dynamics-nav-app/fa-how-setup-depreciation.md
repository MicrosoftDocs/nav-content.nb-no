---
title: Definere avskrivning av aktiva
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 7efc50c673514498de0caa5b3a2dc4b32d4f7f5d
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-depreciation"></a>Definere avskrivning av aktiva
 Du kan bruke ulike avskrivningsmetoder når du skal forberede regnskapsoppgjør og selvangivelse. Mange store selskaper bruker lineær avskrivning i sine regnskapsoppgjør ettersom denne avskrivningsmetoden vanligvis tillater rapportering av høyere inntjening. Når det gjelder inntektsskatt, bruker imidlertid mange virksomheter en hurtig avskrivningsmetode. Hvis du vil ha mer informasjon, kan du se [Avskrivningsmetoder](fa-depreciation-methods.md).

 Når du har opprettet de relevante avskrivningstablåene, må du tilordne minst ett avskrivningstablå til hvert enkelt aktiva. Et avskrivningstablå som tilordnes til et aktiva, blir referert til som et avskrivningstablå for aktiva. Tilsvarende kalles vinduet for tilordnede avskrivningstablåer **Aktivaavskrivningstablå**.

## <a name="to-create-a-depreciation-book"></a>Slik oppretter du et avskrivningstablå:  
I et aktivaavskrivningstablå angir du hvordan aktiva skal avskrives. Hvis du vil tilpasse ulike avskrivningsmetoder, kan du definere flere avskrivningstablåer.  
1.  I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Avskrivningstablåer** og velger deretter den relaterte koblingen.
2. I vinduet **Avskrivningstablå - oversikt** velger du handlingen **Ny**.
3. I vinduet **Avskrivningstablåkort** fyller du ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

    **Merk**: Du kan registrere aktivatransaksjoner i vinduet **Aktivafinanskladd** eller **Aktivakladd**, avhengig av om transaksjonene er for finansiell rapportering eller intern håndtering. Følg neste trinn for å definere hvilken type kladd som brukes for de ulike aktivaaktivitetene som standard.
4. I **Integrasjon**-hurtigfanen merker du av for hver aktivaaktivitet som har transaksjoner du vil bokføre ved hjelp av **Aktivafinanskladd**-vinduet.
5. Gjenta trinn 2 til 4 for hver avskrivningsmetode eller bokføringsmetode som du vil tilordne til aktiva som et avskrivningstablå.

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>Slik tilordner du et avskrivningstablå til et aktiva:  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.
2. Velg aktivaet som du vil definere et aktivaavskrivningstablå for.
3. På hurtigfanen **Avskrivningstablå** fyller du ut feltene etter behov.
4. Hvis du vil tilordne mer enn ett avskrivningstablå til aktivaet, velger du **Legg til flere avskrivningstablåer**.
5. Du kan også velge handlingen **Avskrivningstablåer** for å angi ett eller flere avskrivningstablåer for aktiva.

**Merk**: Når du bruker den manuelle avskrivningsmetoden, må du angi avskrivning manuelt i aktivafinanskladden. Funksjonen **Beregn avskrivninger** utelater aktiva som avskrives etter den manuelle metoden. Du kan bruke denne metoden for aktiva som ikke skal avskrives, for eksempel tomter.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>Slik tilordner du et avskrivningstablå til flere aktiva med en kjørsel:
Hvis du vil tilordne et avskrivningstablå til flere aktiva, kan du bruke kjørselen **Opprett aktivaavskr.tablåer** for å angi at Dynamics NAV automatisk skal opprette de nødvendige aktivaavskrivningstablåene.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.
2. Velg aktivaet som du vil tilordne et avskrivningstablå til, og velg deretter **Rediger**-handlingen.
3. I **Avskrivningstablåkort**-vinduet velger du **Opprett aktivaavskr.tablåer**.
4. I vinduet **Opprett aktivaavskr.tablåer** fyller du ut **Avskrivningstablå**-feltet.
5. Velg feltet**Kopier fra aktivanr.**. Velg deretter aktivanummeret du vil bruke som grunnlag for å opprette nye aktivaavskrivningstablåer.

    Hvis du fyller ut dette feltet, vil avskrivningsfeltene i de nye aktivaavskrivningstablåene inneholde samme informasjon som de tilsvarende feltene i aktivaavskrivningstablået du kopierer fra. La feltet stå tomt hvis du vil opprette nye aktivaavskrivningstablåer med tomme avskrivningsfelt.  
6. På hurtigfanen **Aktiva** kan du definere et filter for å velge hvilke aktiva du vil det skal opprettes aktivaavskrivningstablåer for.
7. Velg **OK**-knappen.

## <a name="to-set-up-depreciation-posting-types"></a>Slik definerer du bokføringstyper for avskrivning:  
For hvert avskrivningstablå må du definere hvordan du vil at Dynamics NAV skal håndtere ulike bokføringstyper. Du må for eksempel angi om bokføringen skal være debet eller kredit, og om bokføringstypen skal tas med i avskrivningsgrunnlaget.  
1.  I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Avskrivningstablåer** og velger deretter den relaterte koblingen.  
2. Velg avskrivningstablået du vil definere, og velg deretter handlingen **Aktivabokf.type - oppsett**.
3. Fyll ut resten av feltene i vinduet **Aktivabokf.type - oppsett** etter behov.

**Merk**: Du kan ikke sette inn eller slette linjer i vinduet **Aktivabokf.type - oppsett**. Du kan bare foreta endringer i de eksisterende linjene.

Vi anbefaler at du ikke endrer oppsettet av avskrivningstablåer med poster som allerede er bokført. Endringene påvirker ikke poster som allerede er bokført, noe som ville forårsaket feilaktig statistikk for avskrivningstablåene.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>Slik definerer du standardmaler og kladder for aktivaavskrivning:  
Du kan definere et standardoppsett for maler og kladder for hvert enkelt avskrivningstablå. Du bruker disse standardene til følgende:
- Duplisere linjer fra én kladd til en annen.
- Opprett kladdelinjer ved hjelp av kjørslene **Beregn avskrivning** eller **Indeksreg. aktiva**.
- Duplisere anskaffelseskostnadene i forsikringskladden.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Avskrivningstablåer** og velger deretter den relaterte koblingen.
2. Velg avskrivningstablået du vil definere standardkladder for, og velg deretter handlingen **Aktivakladdoppsett**.
3. Hvis du vil bruke et standardoppsett for alle brukerne, velger du **Bruker-ID**-feltet som skal velges fra vinduet **Brukere**.
4. Velg kladdemalen eller kladden som skal brukes som standard i de andre feltene.

## <a name="see-also"></a>Se også
[Definere aktiva](fa-setup.md)  
[Administrere aktiva](fa-manage.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

