---
title: Definere generell aktivainformasjon
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
ms.openlocfilehash: 8c0e33a78d47ccfbe39a78f81e31b69f61fd4f80
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-general-fixed-assets-information"></a>Definere generell aktivainformasjon
Før du kan behandle aktiva, må du definere standard finanskonti, fordelingsnøkler, kladdemaler og kladder for aktivabokføring og -reklassifisering, og du kan klassifisere aktiva i klasser, for eksempel materielle og immaterielle.

## <a name="to-set-up-general-default-values-for-fixed-assets"></a>Slik definerer du generelle standardverdier for aktiva
Du definerer den generelle virkemåten eller aktivafunksjonaliteten og bilagsnummerserien i **Aktivaoppsett**-vinduet.

1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivaoppsett** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.

## <a name="to-set-up-fixed-asset-posting-groups"></a>Slik definerer du bokføringsgrupper for aktiva:  
Du bokfører grupper for å definere aktivagrupper. Poster for disse bokføringsgruppene bokføres på de samme finanskontiene.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokf.grupper - aktiva** og velger deretter den relaterte koblingen.  
2. Velg handlingen **Ny**.
3. Fyll ut resten av feltene i vinduet **Kort for bokf.grp.- aktiva** etter behov.

    **Merk**: For å sikre at motkontoer for ulike aktivabokføringer settes inn automatisk når du velger handlingen **Sett inn aktivamotkonto** på kladdelinjer, følger du det neste trinnet, basert på oppskrivningsbokføring.
4. I hurtigfanen **Motkonto** i feltet **Motkonto for oppskrivning** velger du til hvilken finanskonto du vil bokføre motposter for oppskrivning.

Hvis du vil ha mer informasjon om hvordan du bruker handlingen **Sett inn aktivamotkonto** på aktivafinanskladdelinjer, kan du se for eksempel [Revaluere aktiva](fa-how-revalue.md).

## <a name="to-set-up-fixed-asset-allocation-keys"></a>Slik definerer du aktivafordelingsnøkler:  
Ved hjelp av brukerdefinerte fordelingsnøkler kan du fordele transaksjoner på ulike avdelinger eller prosjekter. Du kan for eksempel definere en fordelingsnøkkel som fordeler avskrivningskostnader på biler med 35 prosent til administrasjonsavdelingen og 65 prosent til salgsavdelingen. Hvis du vil ha mer informasjon, kan du se [Bruke fordelingsnøkler i finanskladder](ui-how-use-allocation-keys-general-journals.md).

Fordelingsnøkler gjelder for aktivaklasser, ikke for individuelle aktiva.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokf.grupper - aktiva** og velger deretter den relaterte koblingen.  
2. I vinduet **Bokf.grupper - aktiva** velger du handlingen **Fordelinger**, og velger deretter en bokføringstype.
3. I vinduet **Aktiva - fordelinger** fyller du ut feltene etter behov.
4. Gjenta trinn 2 og 3 for bokføringstypene du vil definere fordelingsnøkler for.

## <a name="to-set-up-fixed-asset-journal-templates"></a>Slik definerer du aktivakladdemaler:  
En mal er et forhåndsdefinert oppsett for en kladd. Malen inneholder opplysninger om sporingskoder, rapporter og nummerserier. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).

Dynamics NAV oppretter automatisk en aktivakladdemal første gang du åpner **Aktivakladd**-vinduet, men du kan definere flere kladdemaler.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivakladdemaler** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov.

## <a name="to-set-up-fixed-asset-journal-batches"></a>Slik definerer du aktivakladder:
Du kan definere flere kladder, som vil si individuelle kladder for hver enkelt kladdemal. Ansatte kan for eksempel ha egne kladder der initialene til de ansatte brukes som kladdenavn. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivakladdemaler** og velger deretter den relaterte koblingen.  
2. Velg den aktuelle kladdemalen, og velg deretter **Kladder**-handlingen.
3. I vinduet **Aktivakladder** fyller du ut feltene etter behov.

## <a name="to-set-up-fixed-asset-reclassification-journal-templates"></a>Slik definerer du aktivareklassifiseringskladdemaler:  
Du kan bruke dedikerte reklassifiseringskladder når du skal overføre, dele opp og knytte sammen aktiva. Dynamics NAV oppretter automatisk en aktivareklassifiseringskladdemal første gang du åpner **Aktivareklass.kladd**-vinduet, men du kan definere flere reklassifiseringskladdemaler. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivareklass.kladdemaler** og velger deretter den relaterte koblingen.  
2. Fyll ut feltene etter behov.

## <a name="to-set-up-fixed-asset-reclassification-journal-batches"></a>Slik definerer du aktivareklassifiseringskladder:  
Du kan definere flere kladder, som vil si individuelle kladder for hver reklassifiseringskladd. Ansatte kan for eksempel ha egne kladder for reklassifisering der initialene til den ansatte brukes som reklassifiseringskladdenavn. Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivareklass.kladdemaler** og velger deretter den relaterte koblingen.  
2. Velg den aktuelle kladdemalen, og velg deretter **Kladder**-handlingen.
3. I vinduet **Aktivareklass.kladder** fyller du ut feltene etter behov.

## <a name="to-set-up-fixed-asset-class-codes"></a>Slik definerer du aktivaklassekoder:  
Aktivaklassekoder kan brukes til å gruppere aktiva, for eksempel i materielle og immaterielle aktiva.
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivaklasser** og velger deretter den relaterte koblingen.
2. Angi koder og navn for klassene du vil opprette.

## <a name="to-set-up-fixed-asset-subclass-codes"></a>Slik definerer du aktivaunderklassekoder:
Du bruker aktivaunderklassekodene til å gruppere aktiva i kategorier, for eksempel bygninger, kjøretøy, møbler eller maskiner.  
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivaunderklasser** og velger deretter den relaterte koblingen.
2. Angi koder og navn for klassene du vil opprette.

## <a name="to-set-up-fixed-asset-location-codes"></a>Slik definerer du aktivalokasjonskoder:
Du bruker aktivalokasjonskoder til å registrere aktivalokasjonen, for eksempel salgsavdeling, resepsjon, administrasjon, produksjon eller lager. Denne informasjonen er nyttig for forsikrings- og lagerformål.
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Aktivalokasjoner** og velger deretter den relaterte koblingen.
2. Angi koder og navn for aktivalokasjonene du vil opprette.

## <a name="to-register-opening-entries"></a>Slik registrerer du åpningsposter  
Hvis du bruker aktiva i Dynamics NAV for første gang, må du først definere modulen Finans før du kan definere aktiva. Hvordan du gjør dette, avhenger av om aktiva er integrert med finans.  

 Bruk følgende fremgangsmåte hvis aktivatransaksjoner skal bokføres i Finans.  

1. Kontroller at du har fullført grunnleggende prosedyrer for oppsett av aktiva.  
2. Opprett et aktivakort for hvert eksisterende aktiva.  
3. Definer aktivaavskrivningstablåer.  
4. Aktiver integrering med Finans ved å følge de neste trinnene.
5. Skriv inn **Avskrivningstablåer** i **Søk**-boksen, og velg deretter den relaterte koblingen.  
6. Velg det aktuelle avskrivningstablået. I fanebladet **Hjem**, under **Behandle**, velger du **Rediger liste** for å åpne **Avskrivningstablåkort**-vinduet.
7. På hurtigfanen **Integrering** må du kontrollere at alle feltene er tomme ved å fjerne alle haker. Hvis du har mer enn ett avskrivningstablå, aktiverer du integrasjon med Finans for hvert enkelt tablå.  
8. Skriv inn følgende linjer for hvert aktivum i aktivakladden:
    - En linje med anskaffelseskosten.
    - En linje med den akkumulerte avskrivningen til slutten av forrige regnskapsår.
    - En linje med den akkumulerte avskrivningen fra begynnelsen av gjeldende regnskapsår til datoen som Dynamics NAV er satt til å starte beregningen av avskrivningen.

Hvis du har andre åpningsbalanser, kan du også oppgi disse nå, for eksempel nedskrivning\- og oppskrivning.  

Hvis ikke aktivaene er integrert med Finans, utelater du trinn 4 til 7.

## <a name="see-also"></a>Se også
[Definere aktiva](fa-setup.md)  
[Administrere aktiva](fa-manage.md)  
[Finans](finance-setup.md)  
[Velkommen til Dynamics NAV](across-get-started.md)

