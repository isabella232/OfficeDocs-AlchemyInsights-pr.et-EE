---
title: Windowsi mäludiagnostika käivitamine opsüsteemis Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826663"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="35f4f-102">Windowsi mäludiagnostika käivitamine opsüsteemis Windows 10</span><span class="sxs-lookup"><span data-stu-id="35f4f-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="35f4f-103">Kui Windows ja teie arvutis olevad rakendused krahhivad, külmutavad või käituvad ebastabiilselt, võib teil olla probleeme arvuti mäluga (RAM).</span><span class="sxs-lookup"><span data-stu-id="35f4f-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="35f4f-104">Windowsi mäludiagnostika abil saate kontrollida arvuti muutmäluga seotud probleeme.</span><span class="sxs-lookup"><span data-stu-id="35f4f-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="35f4f-105">Tippige tegumiriba otsinguväljale mäludiagnostika ja seejärel valige **Windowsi mäludiagnostika**. </span><span class="sxs-lookup"><span data-stu-id="35f4f-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="35f4f-106">Diagnostika käivitamiseks peab arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="35f4f-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="35f4f-107">Saate kohe taaskäivitada (salvestage oma töö ja sulgege esmalt avatud dokumendid ja meilisõnumid) või ajastada diagnostika automaatseks käivitamiseks järgmisel arvuti taaskäivitamisel.</span><span class="sxs-lookup"><span data-stu-id="35f4f-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windowsi mäludiagnostika](media/windows-memory-diagnostic.png)

<span data-ttu-id="35f4f-109">Kui arvuti taaskäivitub, käivitub **Windowsi mäludiagnostika** tööriist automaatselt.</span><span class="sxs-lookup"><span data-stu-id="35f4f-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="35f4f-110">Olek ja edenemine kuvatakse diagnostika käivitamiseks ning teil on võimalus diagnostika tühistada, kui vajutate **klaviatuuril paoklahvi (ESC).**</span><span class="sxs-lookup"><span data-stu-id="35f4f-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="35f4f-111">Kui diagnostika on lõpule viidud, käivitub Windows tavapäraselt.</span><span class="sxs-lookup"><span data-stu-id="35f4f-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="35f4f-112">Kohe pärast taaskäivitamist kuvatakse töölaua kuvamisel teatis (tegumiribal tegevuskeskuse ikooni kõrval), mis näitab, kas mälutõrgei leiti. </span><span class="sxs-lookup"><span data-stu-id="35f4f-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="35f4f-113">Näide.</span><span class="sxs-lookup"><span data-stu-id="35f4f-113">For example:</span></span>

<span data-ttu-id="35f4f-114">Tegevuskeskuse ikoon on järgmine.</span><span class="sxs-lookup"><span data-stu-id="35f4f-114">Here's the Action Center icon:</span></span> ![Tegevuskeskuse ikoon](media/action-center-icon.png) 

<span data-ttu-id="35f4f-116">Ja näidisteatis:</span><span class="sxs-lookup"><span data-stu-id="35f4f-116">And a sample notification:</span></span> ![Mälutõrgeteta](media/no-memory-errors.png)

<span data-ttu-id="35f4f-118">Kui te ei saanud teatist, saate tegevuskeskuse kuvamiseks  ja teatiste keritava loendi kuvamiseks valida tegumiribal tegevuskeskuse ikooni. </span><span class="sxs-lookup"><span data-stu-id="35f4f-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="35f4f-119">Üksikasjaliku teabe läbivaatamiseks tippige **sündmus** tegumiriba otsinguväljale ja seejärel valige **Sündmusevaatur**.</span><span class="sxs-lookup"><span data-stu-id="35f4f-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="35f4f-120">Liikuge **sündmusevaaturi** vasakpoolsel paanil lehele **Windowsi logid ja > System**.</span><span class="sxs-lookup"><span data-stu-id="35f4f-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="35f4f-121">Otsige parempoolsel paanil loendit allapoole, vaadates veergu Allikas, **kuni** näete sündmusi, mille väärtus **on MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="35f4f-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="35f4f-122">Tõstke iga selline sündmus esile ja vaadake tulemiteavet loendi all **vahekaardi Üldist** väljal.</span><span class="sxs-lookup"><span data-stu-id="35f4f-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
