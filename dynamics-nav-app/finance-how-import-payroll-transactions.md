---
title: "Lese inn lønnstransaksjoner"
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: nb-no
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="9d278-102">Lese inn lønnstransaksjoner</span><span class="sxs-lookup"><span data-stu-id="9d278-102">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="9d278-103">For å ta høyde for lønnsutbetalinger og relaterte transaksjoner, må du importere og bokføre finansielle transaksjoner som er utført av lønnssystemet til Finans.</span><span class="sxs-lookup"><span data-stu-id="9d278-103">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="9d278-104">Hvis du vil gjøre dette, importerer du først en CSV-fil.</span><span class="sxs-lookup"><span data-stu-id="9d278-104">To do this, you first import a csv.</span></span> <span data-ttu-id="9d278-105">filen som du mottar fra lønnssystemet til vinduet **Finanskladd**.</span><span class="sxs-lookup"><span data-stu-id="9d278-105">file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="9d278-106">Deretter tilordner du eksterne kontoer i lønnsfilen til de relevante finanskontiene.</span><span class="sxs-lookup"><span data-stu-id="9d278-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="9d278-107">Til slutt kan du bokføre lønnstransaksjoner etter kontotilordningen.</span><span class="sxs-lookup"><span data-stu-id="9d278-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="9d278-108">Slik importerer du en lønnsfil</span><span class="sxs-lookup"><span data-stu-id="9d278-108">To import a payroll file</span></span>
1. <span data-ttu-id="9d278-109">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladder** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="9d278-109">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="9d278-110">I den aktuelle finanskladden velger du handlingen **Importer lønnstransaksjoner**.</span><span class="sxs-lookup"><span data-stu-id="9d278-110">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span>
3. <span data-ttu-id="9d278-111">I vinduet **Importer** velger du den aktuelle lønnsfilen, og deretter velger du **OK**-knappen.</span><span class="sxs-lookup"><span data-stu-id="9d278-111">In the **Import** window, select the relevant payroll file, and then choose the **OK** button.</span></span> <span data-ttu-id="9d278-112">Filen må være i CSV-format.</span><span class="sxs-lookup"><span data-stu-id="9d278-112">The file must be in CSV format.</span></span> 
4. <span data-ttu-id="9d278-113">Følg trinnene i vinduet **Importer lønnstransaksjoner** for å importere transaksjoner og tilordne forretningsforbindelser, og velg deretter **Fullfør**.</span><span class="sxs-lookup"><span data-stu-id="9d278-113">Follow the steps in the **Import Payroll Transactions** window to import transactions and map accounts, and then choose the **Finish** button.</span></span>

    <span data-ttu-id="9d278-114">Økonomijournalen er fylt med linjer som representerer transaksjoner der lønnsfilen og relevante kontiene i kolonnen **Finanskonto**.</span><span class="sxs-lookup"><span data-stu-id="9d278-114">The general journal is filled with lines representing the transactions that the payroll file contains and with the relevant accounts in the **G/L Account** column.</span></span>
4. <span data-ttu-id="9d278-115">Rediger eller bokfør kladdelinjene som for andre transaksjoner i Finans.</span><span class="sxs-lookup"><span data-stu-id="9d278-115">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="9d278-116">Hvis du vil ha mer informasjon, kan du se [Arbeide med finanskladder](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="9d278-116">For more information, see [How to: Work With General Journals](ui-work-general-journals.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="9d278-117">Se også</span><span class="sxs-lookup"><span data-stu-id="9d278-117">See Also</span></span>
[<span data-ttu-id="9d278-118">Finans</span><span class="sxs-lookup"><span data-stu-id="9d278-118">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="9d278-119">Arbeide med finanskladder</span><span class="sxs-lookup"><span data-stu-id="9d278-119">How to: Work With General Journals</span></span>](ui-work-general-journals.md)  

