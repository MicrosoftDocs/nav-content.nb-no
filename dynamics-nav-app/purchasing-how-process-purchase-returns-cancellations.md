---
title: Behandle bestillingsreturer eller annulleringer
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 94067fb3d10975c1db29d2e3f1d5d6373fcbf9f2
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-purchase-returns-or-cancellations"></a>Behandle bestillingsreturer eller annulleringer
Hvis du vil returnere varer til leverandøren eller avbryte tjenester du har kjøpt, kan du opprette og bokføre en kjøpskreditnota som angir den ønskede endringen med hensyn til den opprinnelige kjøpsfakturaen. Du kan opprette kjøpskreditnotaen fra den bokførte kjøpsfakturaen for å ta med de riktige opplysningene for kjøpsfakturaen, eller bruke en kopifunksjon.

Vanligvis oppretter du en kjøpskreditnota i relasjon til en kreditnota du har mottatt fra en leverandør. Kjøpskreditnotaen fungerer som den interne dokumentasjonen av kreditnotaprosessen for regnskapsformål.

Endringen kan relateres til alle produktene på den opprinnelige kjøpsfakturaen eller bare noen av produktene. Du kan derfor delvis returnere mottatte varer eller kreve delvis refusjon av mottatte tjenester. I det tilfellet må du redigere informasjon om den kopierte kjøpsfakturaen.

I tillegg til den opprinnelige bokførte kjøpsfakturaen, kan du bruke kjøpskreditnotaen for andre kjøpsdokumenter, for eksempel en annen bokført kjøpsfaktura, fordi du også returnerer varer som leveres med denne fakturaen.

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Opprett en kjøpskreditnota fra en bokført kjøpsfaktura
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kjøpskreditnotaer** og velger deretter den relaterte koblingen.  
2. I vinduet Bokførte **Kjøpsfakturaer** velger du den bokførte kjøpsfakturaen som du vil tilbakeføre, og deretter velger du handlingen **Opprett korrigerende kreditnota**.

    De fleste feltene på kjøpskreditnotahodet fylles ut med informasjon fra den bokførte kjøpsfakturaen. Du kan redigere alle feltene, for eksempel med ny informasjon som gjenspeiler returavtalen.
3. Redigere informasjonen på linjene i henhold til avtalen, for eksempel antall varer som returneres, eller beløpet som skal refunderes.
4. Velg handlingen **Utlign poster**.
5. I vinduet **Utlign leverandørposter** velger du linjen med det bokførte kjøpsdokumentet du vil utligne kjøpskreditnotaen mot, og deretter velger du handlingen **Utlignings-ID**. Nummeret på kjøpskreditnotaen settes inn i feltet **Utlignings-ID**.
6. I feltet **Beløp som skal utlignes** skriver du inn beløpet som du vil utligne hvis mindre enn det opprinnelige beløpet.

    Nederst i vinduet **Utlign leverandørposter** kan du se det totale beløpet som skal utlignes for å tilbakeføre alle involverte poster, nemlig når verdien i **Saldo** -feltet er null.
7. Velg **OK**-knappen. Når du bokfører kjøpskreditnotaen, brukes den på de angitte bokførte kjøpsdokumenter.

    Når du har opprettet eller redigert nødvendige kjøpskreditnotalinjer og ett eller flere programmer er angitt, kan du fortsette med å bokføre kjøpskreditnotaen.
8. Velg handlingen **Bokfør**.

De bokførte kjøpsfakturaene du utligner kreditnotaen mot, er nå tilbakeført. Hvis du allerede har betalt den opprinnelige fakturaen, skal leverandøren nå refundere betalingen til deg. Hvis kreditnotaen bare er en del av produktet på den opprinnelige fakturaen, kan du bare betale det resterende beløpet på den opprinnelige kjøpsfakturaen for å lukke den.

Kjøpskreditnotaen fjernes og erstattes med et nytt dokument i listen over bokførte kjøpskreditnotaer.

## <a name="to-create-a-purchase-credit-memo-from-scratch"></a>Opprette en kjøpskreditnota fra bunnen av
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Bokførte kjøpsfakturaer** og velger deretter den relaterte koblingen.
2. Velg handlingen **Ny** for å åpne en ny, tom kjøpskreditnota.
3. I feltet **Leverandør** angir du navnet på en eksisterende leverandør.
4. Velg handlingen **Kopier dokument**.
5. Velg **Bokført faktura** i **Bilagstype**-feltet i vinduet **Kopier kjøpsdokument**.
6. Velg **Dokumentnr.** -feltet for å åpne vinduet **Bokførte kjøpsfakturaer**, og velg deretter den bokførte kjøpsfakturaen som inneholder linjer du vil tilbakeføre.
7. Merk av for  **Gjenberegn linjer**  hvis du vil at de kopierte bokførte kjøpsfakturalinjene skal oppdateres med endringer i varepris og enhetskost etter at fakturaen er bokført.
8. Velg **OK**-knappen. De kopierte fakturalinjene settes inn i kjøpskreditnotaen.
9. Fullføre kjøpskreditnotaen som forklart i den avsnittet "Opprette en kjøpskreditnota fra en bokført kjøpsfaktura" i dette emnet.

## <a name="see-also"></a>Se også
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Registrere kjøp](purchasing-how-record-purchases.md)  

