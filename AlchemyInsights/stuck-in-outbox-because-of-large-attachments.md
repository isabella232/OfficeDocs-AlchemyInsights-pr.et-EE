---
title: Takerdunud väljundkasti suurte manuste tõttu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241248"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="94d3b-102">Sõnumite parandamine, mis on väljundkaustas kinni</span><span class="sxs-lookup"><span data-stu-id="94d3b-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="94d3b-103">Soovitame alustada, käivitades stsenaariumi ["Mul on probleeme saatmine, vastuvõtmine või leidmine"](https://aka.ms/SaRA-OutlookSendReceive) [Microsofti toe ja taastamise abimees](https://diagnostics.office.com/#/) tööriista.</span><span class="sxs-lookup"><span data-stu-id="94d3b-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="94d3b-104">Kui sõnum jääb teie väljundkaustas kinni, on kõige tõenäolisem põhjus suur manus või suvand "saada kohe, kui see on ühendatud" pole lubatud.</span><span class="sxs-lookup"><span data-stu-id="94d3b-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="94d3b-105">**Eemaldage suur manus**</span><span class="sxs-lookup"><span data-stu-id="94d3b-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="94d3b-106">Outlookis valige **saatmise/vastuvõtu** > **töö ühenduseta**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="94d3b-107">Valige navigeerimispaanil suvand **Väljundboks**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="94d3b-108">Siit saate:</span><span class="sxs-lookup"><span data-stu-id="94d3b-108">From here, you can:</span></span> 
    - <span data-ttu-id="94d3b-109">Kustutage sõnum (valige see ja seejärel valige **Kustuta**).</span><span class="sxs-lookup"><span data-stu-id="94d3b-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="94d3b-110">Lohistage sõnum mustandite kausta, topeltklõpsake selle avamiseks ja manuse eemaldamiseks valige see ja seejärel valige **Kustuta**).</span><span class="sxs-lookup"><span data-stu-id="94d3b-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="94d3b-111">Kui kuvatakse tõrketeade, mis ütleb, et Outlook proovib sõnumit edastada, sulgege Outlook.</span><span class="sxs-lookup"><span data-stu-id="94d3b-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="94d3b-112">Väljumiseks võib kuluda mõni hetk.</span><span class="sxs-lookup"><span data-stu-id="94d3b-112">It may take a few moments to exit.</span></span> <span data-ttu-id="94d3b-113">Kui Outlook ei sulge, vajutage klahvikombinatsiooni CTRL + ALT + DELETE ja valige **Käivita Tegumihaldur**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="94d3b-114">Valige Tegumihalduris vahekaart **protsessid** , kerige allapoole Outlook. exe ja valige **Lõpeta protsess**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="94d3b-115">Pärast Outlooki sulgemist taaskäivitage see ja korrake juhiseid 2 ja 3.</span><span class="sxs-lookup"><span data-stu-id="94d3b-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="94d3b-116">Pärast manuse eemaldamist klõpsake nuppu **Saada/võta vastu** > **Tööta ühenduseta** , et jätkata töötamist ühendusega.</span><span class="sxs-lookup"><span data-stu-id="94d3b-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="94d3b-117">Sõnumid jäävad ka väljundkasti, kui klõpsate nuppu **saada**, kuid te ei ole ühendatud.</span><span class="sxs-lookup"><span data-stu-id="94d3b-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="94d3b-118">Klõpsake nuppu **Saada/võta vastu** ja vaadake **ühenduseta töö** nuppu.</span><span class="sxs-lookup"><span data-stu-id="94d3b-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="94d3b-119">Kui see on sinine, siis sa oled lahutatud.</span><span class="sxs-lookup"><span data-stu-id="94d3b-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="94d3b-120">Klõpsake seda ühendamiseks (nupp muutub valgeks) ja klõpsake **saada kõik**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="94d3b-121">**Luba saatmine kohe, kui see on ühendatud**</span><span class="sxs-lookup"><span data-stu-id="94d3b-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="94d3b-122">Klõpsake menüü Fail käsku **Suvandid**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="94d3b-123">Klõpsake dialoogiboksis Outlooki suvandid nuppu **Täpsemalt**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="94d3b-124">Klõpsake jaotises saatmise ja vastuvõtu lubamiseks **Saada kohe, kui**see on ühendatud.</span><span class="sxs-lookup"><span data-stu-id="94d3b-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="94d3b-125">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="94d3b-125">Click **OK**.</span></span>
 
<span data-ttu-id="94d3b-126">Täielikud üksikasjad leiate teemast:</span><span class="sxs-lookup"><span data-stu-id="94d3b-126">For full details, see:</span></span>
- [<span data-ttu-id="94d3b-127">Video: saata või kustutada ummikus e-posti</span><span class="sxs-lookup"><span data-stu-id="94d3b-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="94d3b-128">E-posti jääb kausta saatmiseks kuni te käsitsi algatada saatmise/vastuvõtu toiming Outlookis</span><span class="sxs-lookup"><span data-stu-id="94d3b-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
