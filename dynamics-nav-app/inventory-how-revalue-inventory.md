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


# <a name="how-to-revalue-inventory"></a><span data-ttu-id="38bd3-103">Revaluere beholdning</span><span class="sxs-lookup"><span data-stu-id="38bd3-103">How to: Revalue Inventory</span></span>   
<span data-ttu-id="38bd3-104">Hvis du vil endre lagerverdien for en vare eller en bestemt varepost, må du bruke revalueringskladden.</span><span class="sxs-lookup"><span data-stu-id="38bd3-104">If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.</span></span>

## <a name="to-revalue-inventory"></a><span data-ttu-id="38bd3-105">Slik revaluerer du beholdning</span><span class="sxs-lookup"><span data-stu-id="38bd3-105">To revalue inventory</span></span>
1. <span data-ttu-id="38bd3-106">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Revalueringskladd** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="38bd3-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Revaluation Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="38bd3-107">Velg handlingen **Beregn lagerverdi**.</span><span class="sxs-lookup"><span data-stu-id="38bd3-107">Choose the **Calculate Inventory Value** action.</span></span>
3. <span data-ttu-id="38bd3-108">I vinduet **Beregn lagerverdi** fyller du ut feltene etter behov.</span><span class="sxs-lookup"><span data-stu-id="38bd3-108">In the **Calculate Inventory Value** window, fill in the fields as necessary.</span></span> <span data-ttu-id="38bd3-109">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="38bd3-109">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="38bd3-110">Velg **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="38bd3-110">Choose the **OK** button.</span></span>
5. <span data-ttu-id="38bd3-111">På hver linje i vinduet **Revalueringskladd** i feltet **Enhetskost (revaluert)** angir du den nye enhetskosten.</span><span class="sxs-lookup"><span data-stu-id="38bd3-111">On each line in the **Revaluation Journal** window, in the **Unit Cost (Revalued)** field, enter the new unit cost.</span></span> <span data-ttu-id="38bd3-112">Du kan eventuelt angi det nye totalbeløpet i feltet **Lagerverdi (revaluert)**.</span><span class="sxs-lookup"><span data-stu-id="38bd3-112">Alternatively, enter the new total amount in the **Inventory Value (Revalued)** field.</span></span>

    <span data-ttu-id="38bd3-113">De relevante feltene oppdateres automatisk.</span><span class="sxs-lookup"><span data-stu-id="38bd3-113">The relevant fields are automatically updated.</span></span> <span data-ttu-id="38bd3-114">Merk deg at feltet **Beløp** viser den faktiske endringen i lagerverdien for den vareposten du har valgt.</span><span class="sxs-lookup"><span data-stu-id="38bd3-114">Note that the **Amount** field shows the actual change in inventory value for the selected item ledger entry.</span></span> <span data-ttu-id="38bd3-115">I dette feltet beregnes differansen mellom feltene **Lagerverdi (beregnet)** og **Lagerverdi (revaluert)**.</span><span class="sxs-lookup"><span data-stu-id="38bd3-115">It calculates the difference between the **Inventory Value (Calculated)** field and the **Inventory Value (Revalued)** field.</span></span>

6. <span data-ttu-id="38bd3-116">Når du har fullført alle linjene i revalueringskladden, kan du velge handlingen **Bokfør**.</span><span class="sxs-lookup"><span data-stu-id="38bd3-116">When you have completed all lines in the revaluation journal, choose the **Post** action.</span></span>

<span data-ttu-id="38bd3-117">Nye verdiposter opprettes nå for å gjenspeile revalueringer som du har bokført.</span><span class="sxs-lookup"><span data-stu-id="38bd3-117">New value entries are now created to reflect the revaluations that you have posted.</span></span> <span data-ttu-id="38bd3-118">Du kan se de nye verdiene på de respektive varekortene.</span><span class="sxs-lookup"><span data-stu-id="38bd3-118">You can see the new values on the respective item cards.</span></span>

## <a name="see-also"></a><span data-ttu-id="38bd3-119">Se også</span><span class="sxs-lookup"><span data-stu-id="38bd3-119">See Also</span></span>
[<span data-ttu-id="38bd3-120">Håndtere lager</span><span class="sxs-lookup"><span data-stu-id="38bd3-120">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="38bd3-121">Håndtere salg</span><span class="sxs-lookup"><span data-stu-id="38bd3-121">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="38bd3-122">Håndtere kjøp</span><span class="sxs-lookup"><span data-stu-id="38bd3-122">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="38bd3-123">Arbeide med Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="38bd3-123">Work With Dynamics NAV</span></span>](ui-work-product.md)

