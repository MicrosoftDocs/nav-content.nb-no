---
title: Anskaffe aktiva
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
ms.openlocfilehash: 5b58a6cf0a0c22c8076082328f92725cb7dbc4d1
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-acquire-fixed-assets"></a>Anskaffe aktiva
For hvert enkelt aktiva må du definere et kort som inneholder opplysninger om aktivaet. Du kan definere bygninger eller produksjonsutstyr som hovedaktiva i en komponentoversikt, og du kan gruppere dem på forskjellige måter, som etter klasse, avdeling eller lokasjon. Et avskrivningstablå må defineres og tilordnes til hvert enkelt aktiva før du kan anskaffe det.

Når et aktiva er definert og et avskrivningstablå tilordnet, må du anskaffe det. For å anskaffet et aktiva registrerer du anskaffelseskosten i den relevante finanskontoen, bankkontoen eller leverandøren ved å bokføre en anskaffelsestransaksjon fra **Aktiva finanskladd**-vinduet. Du kan bruke **Assistert aktivaanskaffelse**-vinduet for å opprette og bokføre de nødvendige finanskladdelinjene automatisk.

Skrapverdien er restverdien for et aktiva som ikke lenger kan brukes. Du kan bokføre skrapverdien samtidig som du bokfører anskaffelseskosten. Hvis du vil ha mer informasjon, se [Avskrive eller amortisere aktiva](fa-how-depreciate-amortize.md).

Indeksregulering brukes til å justere verdier for generelle endringer i prisnivået. Kjørselen **Indeksreg. aktiva** kan brukes til å beregne anskaffelseskostnader i forbindelse med gjenskaffelseskostnader.

## <a name="to-create-a-fixed-asset-and-acquire-it-automatically"></a>Slik oppretter du et anleggsmiddel og anskaffer det automatisk:
Følgende fremgangsmåte beskriver hvordan du oppretter et aktiva og deretter anskaffer det ved hjelp av **Assistert aktivaanskaffelse**-vinduet for å opprette og bokføre de nødvendige aktivafinanskladdelinjene. Du kan også opprette og bokføre kladdelinjene manuelt. Hvis du vil ha mer informasjon, se "Slik bokfører du en aktivaanskaffelse manuelt med aktivafinanskladden".

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.  
2. Velg **Ny**, og deretter fyller du ut feltene i **Generelt**-hurtigfanen etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. På hurtigfanen **Avskrivningstablå** fyller du ut feltene etter behov. Dette trinnet tilordner et avskrivningstablå til aktivaet.  
4. Hvis du vil tilordne mer enn ett avskrivningstablå til aktivaet, velger du **Legg til flere avskrivningstablåer**. Hvis du vil ha mer informasjon, se "Slik tilordner du et avskrivningstablå til et aktiva" i [Definere avskrivningstablåer for aktiva](fa-how-setup-depreciation.md).

    Når alle nødvendige felt for å anskaffe et anleggsmiddel er fylt ut, vises varselet **Du er klar til å anskaffe aktivaet** øverst på siden.
5. Velg handlingen **Anskaffe** i varselet.
6. Følg trinnene i **Assistert aktivaanskaffelse**-vinduet for å fullføre den automatiske anskaffelsen av aktivaet.

**Merk**: Du kan også bokføre anskaffelseskosten som et kreditbeløp. Husk i så fall at verdien i **Anskaffelseskost inkl. mva**-feltet må ha et minustegn for å angi et kreditbeløp.

Når du velger **Fullfør**, blir **Bokført verdi**-feltet i **Aktivakort**-vinduet fylt ut, som indikerer at aktivaet er anskaffet til den angitte anskaffelseskosten.  

## <a name="to-set-up-a-component-list-for-a-main-asset"></a>Slik definerer du en komponentoversikt for et hovedaktiva:  
Du kan gruppere aktiva i hovedaktiva og komponenter i hovedaktivaene. Det kan for eksempel tenkes at du har en produksjonsmaskin som består av mange deler som du vil gruppere på denne måten.  

Både hovedaktivaet og alle komponentene må defineres som individuelle aktivakort. Når du har definert en komponentoversikt, fylles feltene **Hovedaktiva/komponent** og **Komponent til hovedaktiva** automatisk ut på aktivakortene.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktiva** og velger deretter den relaterte koblingen.
2. Velg aktivaet som er hovedaktivaet, og velg deretter **Hovedaktivakomponenter**-handlingen.
3. I **Hovedaktivakomponenter**-vinduet velger du **Aktivanr.**-feltet og velger deretter aktivaet som du vil legge til som en komponent i hovedaktivaet.
4. Lukk vinduet.
5. Gjenta trinnene 3 og 4 for hvert komponentaktiva som du vil legge til.
6. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivaoppsett** og velger deretter den relaterte koblingen.
7. Merk av for **Tillat bokf. til hovedaktiva**.

## <a name="to-post-a-fixed-asset-acquisition-manually-with-the-fixed-asset-gl-journal"></a>Slik bokfører du en aktivaanskaffelse manuelt med aktivafinanskladden:
Følgende fremgangsmåte beskriver hvordan du anskaffer et aktiva manuelt ved å opprette og bokføre linjer i **Aktiva finanskladd**-vinduet. Du kan også anskaffe et aktiva automatisk ved hjelp av **Assistert aktivaanskaffelse**-vinduet. Hvis du vil ha mer informasjon, kan du se trinn 5 i "Slik oppretter du et anleggsmiddel og anskaffer det automatisk".

**Merk**: Du kan også bokføre anskaffelseskosten som et kreditbeløp. Husk i så fall at verdien i **Beløp**-feltet må ha et minustegn for å angi et kreditbeløp.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivafinanskladder** og velger deretter den relaterte koblingen.
2. I **Aktiva finanskladd**-vinduet i **Aktivabokf.type**-feltet velger du **Anskaffelseskost**.
3. Fyll ut feltene som gjenstår etter behov.
4. Velg handlingen **Bokfør**.  

**Tips**: Hvis du fyller ut **Forsikringsnr.**-feltet i aktivafinanskladden når du bokfører en anskaffelseskost, bokføres også anskaffelseskosten for aktivaet i forsikringsdekningsposten. Hvis du vil ha mer informasjon, se [Forsikre aktiva](fa-how-insure.md).

## <a name="to-cancel-an-acquisition-cost-posting-for-one-fixed-asset"></a>Slik kansellerer du en anskaffelseskostbokføring for ett aktiva:
Hvis du gjør en feil når du bokfører en anskaffelseskostnad, kan du fjerne posten via kjørselen **Kanseller aktivaposter** og deretter bokføre den riktige anskaffelsesposten. Feilaktige poster overføres til **Aktivafeilposter**-vinduet.

For eksempel hvis du bokfører en anskaffelse med feil dato, må du korrigere den så snart som mulig fordi aktivabokføringsdatoen brukes i mange viktige beregninger.

**Viktig**: Du kan ikke bruke **Tilbakefør transaksjon**-funksjonen for aktivaposter.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kanseller aktivaposter** og velger deretter den relaterte koblingen.
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
3. Velg **OK**-knappen for å kjøre kjørselen.
4. Når feil post eller poster er kansellert, fortsetter du med å bokføre riktig anskaffelseskost.

Hvis du vil kansellere finansposter for flere aktiva samtidig, kan du bruke **Kanseller aktivaposter**-kjørselen.

## <a name="to-post-the-salvage-value-together-with-the-acquisition-cost"></a>Slik bokfører du skrapverdien sammen med anskaffelseskosten:  
Du kan bokføre skrapverdien sammen med anskaffelseskosten fra en aktivafinanskladd.    

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kanseller aktivaposter** og velger deretter den relaterte koblingen.
2. Opprett anskaffelseskladdelinjen. Hvis du vil ha mer informasjon, se "Slik bokfører du en aktivaanskaffelse manuelt med aktivafinanskladden".
3. I **Skrapverdi**-feltet på kladdelinjen angir du beløpet for skrapverdien som et kreditbeløp (med et minustegn).
4. Velg handlingen **Bokfør**.

**Merk**: Bokføringstypen **Skrapverdi** er et alternativ som bare finnes i **Aktivakladd**-vinduet. Det er ikke tilgjengelig i **Aktiva finanskladd**-vinduet fordi skrapverdien ikke bokføres i Finans.

## <a name="see-also"></a>Se også
[Administrere aktiva](fa-manage.md)  
[Definere aktiva](fa-setup.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

