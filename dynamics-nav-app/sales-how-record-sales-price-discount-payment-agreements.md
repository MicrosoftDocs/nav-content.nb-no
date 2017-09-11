---
title: Registrere salgspriser og rabatter
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 80a0ac1edc994f44795f7f907a647b269578bc47
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a><span data-ttu-id="9a6b8-102">Registrere salgspriser og rabatter</span><span class="sxs-lookup"><span data-stu-id="9a6b8-102">How to: Record Sales Prices and Discounts</span></span>
<span data-ttu-id="9a6b8-103">De ulike pris- og rabattavtalene som gjelder ved salg til ulike kunder, må defineres slik at de avtalte reglene og verdiene brukes på salgsdokumenter du oppretter for kundene.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-103">The different price and discount agreements that apply when selling to different customers must be defined so that the agreed rules and values are applied to sales documents that you create for the customers.</span></span>

<span data-ttu-id="9a6b8-104">Når det gjelder priser, kan du sette inn en spesialsalgspris på salgslinjer hvis en bestemt kombinasjon av kunde, vare, minste antall, enhet, eller start-/sluttdato finnes.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-104">Concerning prices, you can have a special sales price inserted on sales lines if a certain combination of customer, item, minimum quantity, unit of measure, or starting/ending date exists.</span></span>

<span data-ttu-id="9a6b8-105">Når det gjelder rabatter, kan du opprette og bruke to typer salgsrabatter:</span><span class="sxs-lookup"><span data-stu-id="9a6b8-105">Concerning discounts, you can set up and use two types of sales discounts:</span></span>

|<span data-ttu-id="9a6b8-106">Rabattype</span><span class="sxs-lookup"><span data-stu-id="9a6b8-106">Discount Type</span></span> |<span data-ttu-id="9a6b8-107">Beskrivelse</span><span class="sxs-lookup"><span data-stu-id="9a6b8-107">Description</span></span> |
|--------------|------------|
|<span data-ttu-id="9a6b8-108">**Salgslinjerabatt**</span><span class="sxs-lookup"><span data-stu-id="9a6b8-108">**Sales Line Discount**</span></span>|<span data-ttu-id="9a6b8-109">Et rabattbeløp som settes inn på salgslinjer hvis en bestemt kombinasjon av kunde, vare, minste antall, enhet, eller start-/sluttdato finnes.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-109">An amount discount that is inserted on sales lines if a certain combination of customer, item, minimum quantity, unit of measure, or starting/ending date exists.</span></span> <span data-ttu-id="9a6b8-110">Dette fungerer på samme måte som for salgspriser.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-110">This works in the same way as for sales prices.</span></span>|
|<span data-ttu-id="9a6b8-111">**Fakturarabatt**</span><span class="sxs-lookup"><span data-stu-id="9a6b8-111">**Invoice Discount**</span></span>|<span data-ttu-id="9a6b8-112">En prosentrabatt som trekkes fra dokumenttotalen hvis beløpet for alle linjer på et salgsdokument overskrider et bestemt minimumsbeløp.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-112">A percentage discount that is subtracted from the document total if the value amount of all lines on a sales document exceeds a certain minimum.</span></span>|

<span data-ttu-id="9a6b8-113">Ettersom salgspriser og salgslinjerabatter er basert på en kombinasjon av vare og kunde, kan du også utføre denne konfigurasjon fra varekortet for varen der reglene og verdiene skal brukes.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-113">Because sales prices and sales line discounts are based on a combination of item and customer, you can also perform this configuration from the item card of the item where the rules and values apply.</span></span>

## <a name="to-set-up-a-sales-price-for-a-customer"></a><span data-ttu-id="9a6b8-114">Definere salgspriser for en kunde</span><span class="sxs-lookup"><span data-stu-id="9a6b8-114">To set up a sales price for a customer</span></span>
1. <span data-ttu-id="9a6b8-115">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kunder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-115">In the top right corner, choose the **Search for Page or Report** icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="9a6b8-116">Åpne det aktuelle kundekortet, og velg deretter handlingen **Priser**.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-116">Open the relevant customer card, and then choose the **Prices** action.</span></span>

    <span data-ttu-id="9a6b8-117">Feltet **Salgstype** er forhåndsutfylt med **Kunde**, og feltet **Salgskode** er forhåndsutfylt med kundenummeret.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-117">The **Sales Type** field is prefilled with **Customer**, and the **Sales Code** field is prefilled with the customer number.</span></span>
3. <span data-ttu-id="9a6b8-118">Fyll ut feltene på linjen etter behov.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-118">Fill in the fields on the line as necessary.</span></span> <span data-ttu-id="9a6b8-119">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-119">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="9a6b8-120">Fyll ut en linje for hver kombinasjon som gir en spesialsalgspris for kunden.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-120">Fill a line for each combination that will grant a special sales price to the customer.</span></span>

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a><span data-ttu-id="9a6b8-121">Definere en salgslinjerabatt for en kunde</span><span class="sxs-lookup"><span data-stu-id="9a6b8-121">To set up a sales line discount for a customer</span></span>
1. <span data-ttu-id="9a6b8-122">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kunder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-122">In the top right corner, choose the **Search for Page or Report** icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="9a6b8-123">Åpne det aktuelle kundekortet, og velg deretter handlingen **Linjerabatter**.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-123">Open the relevant customer card, and then choose the **Line Discounts** action.</span></span>

    <span data-ttu-id="9a6b8-124">Feltet **Salgstype** er forhåndsutfylt med **Kunde**, og feltet **Salgskode** er forhåndsutfylt med kundenummeret.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-124">The **Sales Type** field is prefilled with **Customer**, and the **Sales Code** field is prefilled with the customer number.</span></span>
3.  <span data-ttu-id="9a6b8-125">Fyll ut feltene på linjen etter behov.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-125">Fill in the fields on the line as necessary.</span></span> <span data-ttu-id="9a6b8-126">Velg et felt som skal inneholde en kort beskrivelse av feltet eller kobling til mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-126">Choose a field to read a short description of the field or link to more information.</span></span>
4. <span data-ttu-id="9a6b8-127">Fyll ut en linje for hver kombinasjon som gir en salgslinjerabatt for kunden.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-127">Fill a line for each combination that will grant a sales line discount to the customer.</span></span>

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a><span data-ttu-id="9a6b8-128">Definere en fakturarabatt for en kunde</span><span class="sxs-lookup"><span data-stu-id="9a6b8-128">To set up an invoice discount for a customer</span></span>
<span data-ttu-id="9a6b8-129">Når du har bestemt hvilke kunder som skal gis fakturarabatter, angir du fakturarabattkode på kundekortet og definerer betingelsene for hver kode.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-129">When you have decided which customers are eligible for invoice discounts, enter the invoice discount code on the customer cards and set up the terms for each code.</span></span>

1. <span data-ttu-id="9a6b8-130">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Kunder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="9a6b8-131">Åpne kundekortet for kunden som skal ha fakturarabatter.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-131">Open the customer card for a customer that will be eligible for invoice discounts.</span></span>
3. <span data-ttu-id="9a6b8-132">I feltet **Fakturarabattkode** velger du en kode for de aktuelle fakturarabattbetingelsene som skal brukes til å beregne fakturarabatter for kunden.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-132">In the **Invoice Disc. Code** field, select a code for the relevant invoice discount terms to use to calculate invoice discounts for the customer.</span></span>

    <span data-ttu-id="9a6b8-133">**Merk**: Fakturarabattkoder representeres av eksisterende kundekort.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-133">**Note**: Invoice discount codes are represented by existing customer cards.</span></span> <span data-ttu-id="9a6b8-134">Dette lar deg raskt tilordne fakturarabattbetingelsene til kunder ved å velge navnet på en annen kunde som har de samme betingelsene.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-134">This enables you to quickly assign invoice discount terms to customers by picking the name of another customer who will have the same terms.</span></span>

    <span data-ttu-id="9a6b8-135">Fortsett å definere nye betingelser for salgsfakturarabatt.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-135">Proceed to set up new the sales invoice discount terms.</span></span>
4. <span data-ttu-id="9a6b8-136">I vinduet **Kundekort** velger du handlingen **Fakturarabatter**.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-136">In the **Customer Card** window, choose the **Invoice Discounts** action.</span></span> <span data-ttu-id="9a6b8-137">Vinduet **Kundefakturarabatter** åpnes.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-137">The **Cust. Invoice Discounts** window opens.</span></span>
5. <span data-ttu-id="9a6b8-138">I feltet **Valutakode** angir du koden til en valuta som fakturarabattbetingelsene på linjen gjelder for.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-138">In the **Currency Code** field, enter the code for a currency that the invoice discount terms on the line applies to.</span></span> <span data-ttu-id="9a6b8-139">La feltet stå tomt for å definere betingelser for fakturarabatt i USD.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-139">Leave the field blank to set up invoice discount terms in USD.</span></span>
6. <span data-ttu-id="9a6b8-140">I **Minimumsbeløp**-feltet angir du hva som er minstebeløpet for at det skal gis rabatt i en faktura.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-140">In the **Minimum Amount** field, enter the minimum amount that an invoice must have to be eligible for the discount.</span></span>
7. <span data-ttu-id="9a6b8-141">I **Rabatt-%**-feltet angir du fakturarabatten prosentvis av fakturabeløpet.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-141">In the **Discount %** field, enter the invoice discount as a percentage of the invoice amount.</span></span>
8. <span data-ttu-id="9a6b8-142">Gjenta trinn 5 til 7 for hver valuta som kunden vil motta en forskjellig fakturarabatt for.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-142">Repeat steps 5 through 7 for each currency that the customer will receive a different invoice discount for.</span></span>

<span data-ttu-id="9a6b8-143">Fakturarabatten er nå definert og tilordnet til den aktuelle kunden.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-143">The invoice discount is now set up and assigned to the customer in question.</span></span> <span data-ttu-id="9a6b8-144">Når du velger kundekoden i **Fakturarabattkode**-feltet på andre kundekort, tilordnes den samme fakturarabatten til kundene.</span><span class="sxs-lookup"><span data-stu-id="9a6b8-144">When you select the customer code in the **Invoice Disc. Code** field on other customer cards, the same invoice discount is assigned to those customers.</span></span>

## <a name="see-also"></a><span data-ttu-id="9a6b8-145">Se også</span><span class="sxs-lookup"><span data-stu-id="9a6b8-145">See Also</span></span>  
[<span data-ttu-id="9a6b8-146">Definere salg</span><span class="sxs-lookup"><span data-stu-id="9a6b8-146">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="9a6b8-147">Håndtere salg</span><span class="sxs-lookup"><span data-stu-id="9a6b8-147">Manage Sales</span></span>](sales-manage-sales.md)

