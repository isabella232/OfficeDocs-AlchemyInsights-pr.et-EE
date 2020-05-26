---
title: Windowsi mäludiagnostika käivitamine Windows 10-s
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357515"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="81c07-102">Windowsi mäludiagnostika käivitamine Windows 10-s</span><span class="sxs-lookup"><span data-stu-id="81c07-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="81c07-103">Kui arvuti Windows ja rakendused on krahh, külmutamine või ebastabiilsel viisil tegutsemine, võib teil olla probleem arvuti mäluga (RAM).</span><span class="sxs-lookup"><span data-stu-id="81c07-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="81c07-104">ARVUTI RAM-i probleemide kontrollimiseks saate käivitada Windowsi mäludiagnostika.</span><span class="sxs-lookup"><span data-stu-id="81c07-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="81c07-105">Tippige tegumiriba otsinguväljale tekst **mälu diagnostika**ja seejärel valige **Windowsi mäludiagnostika**.</span><span class="sxs-lookup"><span data-stu-id="81c07-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="81c07-106">Diagnostika käivitamiseks peab arvuti taaskäivitama.</span><span class="sxs-lookup"><span data-stu-id="81c07-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="81c07-107">Teil on võimalus kohe taaskäivitada (salvestage oma töö ja sulgege avatud dokumendid ja e-kirjad kõigepealt) või ajastada diagnostika automaatseks käivitamiseks järgmine kord, kui arvuti taaskäivitub:</span><span class="sxs-lookup"><span data-stu-id="81c07-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windowsi mäludiagnostika](media/windows-memory-diagnostic.png)

<span data-ttu-id="81c07-109">Kui arvuti taaskäivitub, käivitub **Windowsi mälutuvastustööriist** automaatselt.</span><span class="sxs-lookup"><span data-stu-id="81c07-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="81c07-110">Olek ja edenemine kuvatakse diagnostika käivitada, ja teil on võimalus tühistada diagnostika lööb **ESC** klahvi klaviatuuril.</span><span class="sxs-lookup"><span data-stu-id="81c07-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="81c07-111">Kui diagnostika on lõpule jõudnud, hakkab Windows normaalselt käivituma.</span><span class="sxs-lookup"><span data-stu-id="81c07-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="81c07-112">Kohe pärast taaskäivitamist, kui kuvatakse töölaua, kuvatakse teade (kõrval tegumiribal **tegevuskeskuse** ikoon), et näidata, kas mälu tõrked leiti.</span><span class="sxs-lookup"><span data-stu-id="81c07-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="81c07-113">Näiteks.</span><span class="sxs-lookup"><span data-stu-id="81c07-113">For example:</span></span>

<span data-ttu-id="81c07-114">Siin on tegevuskeskuse ikoon:</span><span class="sxs-lookup"><span data-stu-id="81c07-114">Here's the Action Center icon:</span></span> ![Tegevuskeskuse ikoon](media/action-center-icon.png) 

<span data-ttu-id="81c07-116">Ja näidisteatis:</span><span class="sxs-lookup"><span data-stu-id="81c07-116">And a sample notification:</span></span> ![Mälu tõrkeid pole](media/no-memory-errors.png)

<span data-ttu-id="81c07-118">Kui teate vastamata, saate **tegevuskeskuse** kuvamiseks valida tegumiribal **tegevuskeskuse** ikooni ja vaadata teatiste keritav loend.</span><span class="sxs-lookup"><span data-stu-id="81c07-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="81c07-119">Üksikasjaliku teabe läbivaatamiseks tippige **sündmus** tegumiriba otsinguväljale ja seejärel valige **Sündmusevaatur**.</span><span class="sxs-lookup"><span data-stu-id="81c07-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="81c07-120">Liikuge **sündmusevaaturi**vasakpoolsel paanil **Windowsi logid > System**.</span><span class="sxs-lookup"><span data-stu-id="81c07-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="81c07-121">Skannige parempoolsel paanil loendit, vaadates veergu **Allikas** , kuni näete sündmusi, millel on allika väärtuse **memorydiagnostics-tulemused**.</span><span class="sxs-lookup"><span data-stu-id="81c07-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="81c07-122">Tõstke iga selline sündmus esile ja vaadake tulemuste teavet kasti all vahekaardi **Üldine** loendis.</span><span class="sxs-lookup"><span data-stu-id="81c07-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
