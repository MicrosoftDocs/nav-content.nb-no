---
title: "Bokføre avslutningsposten for årsslutt"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: fe32ee973c90ba857852ae092acf03db09e648ee
ms.contentlocale: nb-no
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-post-year-end-closing-entry"></a><span data-ttu-id="dc5b7-102">Bokføre avslutningsposten for årsslutt</span><span class="sxs-lookup"><span data-stu-id="dc5b7-102">How to: Post Year-End Closing Entry</span></span>
<span data-ttu-id="dc5b7-103">Som en del av avslutning av tablåene for et regnskapsår, kjører du kjørselen Lukk resultatregnskapet for å overføre årets resultat til en konto i balansen og lukke resultatregnskapskontiene.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-103">As part of closing the books for a fiscal year, you will run the Close Income Statement batch job to transfer the year's result to an account in the balance sheet and close the income statement accounts.</span></span> <span data-ttu-id="dc5b7-104">Når du kjører den satsvise jobben Lukk resultatregnskapet, må du åpne kladden du angav i kjørselen, og deretter se gjennom og bokføre postene.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-104">After you run the Close Income Statement batch job, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="dc5b7-105">Bokføre avslutningsposten for årsslutt</span><span class="sxs-lookup"><span data-stu-id="dc5b7-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="dc5b7-106">I øvre høyre hjørne velger du ikonet **Søk etter side eller rapport**, angir **Finanskladd** og velger deretter den relaterte koblingen.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-106">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="dc5b7-107">I **Bunkenavn**-feltet i vinduet **Finanskladd**, velger du bunken som inneholder avslutningspostene.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-107">In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="dc5b7-108">Se gjennom postene.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-108">Review the entries.</span></span>
4. <span data-ttu-id="dc5b7-109">Velg handlingen **Bokfør** for å bokføre kladden.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-109">To post the journal, choose the **Post** action.</span></span>

<span data-ttu-id="dc5b7-110">**Merk**: Det vises en feilmelding hvis feil blir oppdaget.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-110">**Note**: If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="dc5b7-111">Hvis bokføringen lykkes, fjernes de bokførte postene fra kladden.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="dc5b7-112">Når bokføringen er fullført, posteres en oppføring på hver resultatregnskapskonto, slik at saldoen blir null og årsresultatet overføres til balansen.</span><span class="sxs-lookup"><span data-stu-id="dc5b7-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="dc5b7-113">Se også</span><span class="sxs-lookup"><span data-stu-id="dc5b7-113">See Also</span></span>
[<span data-ttu-id="dc5b7-114">Lukk bøker</span><span class="sxs-lookup"><span data-stu-id="dc5b7-114">Close Books</span></span>](year-close-books.md)  
[<span data-ttu-id="dc5b7-115">Lukk resultatregnskapet</span><span class="sxs-lookup"><span data-stu-id="dc5b7-115">Close Income Statement</span></span>](year-close-income-statement.md)  
[<span data-ttu-id="dc5b7-116">Lukke regnskapsperioder</span><span class="sxs-lookup"><span data-stu-id="dc5b7-116">How to: Close Accounting Periods</span></span>](year-close-account-periods.md)  
