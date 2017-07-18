<properties
                pageTitle="Revaluere beholdning| Dynamics NAV"
                description="Beskriver hvordan du setter pris på eller avskriver verdien av én eller flere varer på lager ved postering av den gjeldende, beregnede verdien."
                services="project-madeira"
                documentationCenter=""
                authors="SorenGP"
/>
<tags
    ms.service="project-madeira"
    ms.topic="article"
    ms.devlang="na"
    ms.tgt_pltfrm="na"
    ms.workload="na"
    ms.date="11/07/2016"
    ms.author="SorenGP" />


# <a name="how-to-revalue-inventory"></a>Revaluere beholdning   
Hvis du vil endre lagerverdien for en vare eller en bestemt varepost, må du bruke revalueringskladden.

## <a name="to-revalue-inventory"></a>Slik revaluerer du beholdning
1. I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Revalueringskladd** og velger deretter den relaterte koblingen.
2. Velg handlingen **Beregn lagerverdi**.
3. I vinduet **Beregn lagerverdi** fyller du ut feltene etter behov. Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.
4. Velg **OK**-knappen.
5. På hver linje i vinduet **Revalueringskladd** i feltet **Enhetskost (revaluert)** angir du den nye enhetskosten. Du kan eventuelt angi det nye totalbeløpet i feltet **Lagerverdi (revaluert)**.

    De relevante feltene oppdateres automatisk. Merk deg at feltet **Beløp** viser den faktiske endringen i lagerverdien for den vareposten du har valgt. I dette feltet beregnes differansen mellom feltene **Lagerverdi (beregnet)** og **Lagerverdi (revaluert)**.

6. Når du har fullført alle linjene i revalueringskladden, kan du velge handlingen **Bokfør**.

Nye verdiposter opprettes nå for å gjenspeile revalueringer som du har bokført. Du kan se de nye verdiene på de respektive varekortene.

## <a name="see-also"></a>Se også
[Håndtere lager](inventory-manage-inventory.md)  
[Håndtere salg](sales-manage-sales.md)  
[Håndtere kjøp](purchasing-manage-purchasing.md)  
[Arbeide med Dynamics NAV](ui-work-product.md)

