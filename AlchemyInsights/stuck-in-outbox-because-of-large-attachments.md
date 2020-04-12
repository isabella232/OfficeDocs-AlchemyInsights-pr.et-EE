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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232626"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b5ff7-102">Sõnumite parandamine, mis on väljundkaustas kinni</span><span class="sxs-lookup"><span data-stu-id="b5ff7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b5ff7-103">Soovitame alustada, käivitades stsenaariumi ["Mul on probleeme saatmine, vastuvõtmine või leidmine"](https://aka.ms/SaRA-OutlookSendReceive) [Microsofti toe ja taastamise abimees](https://diagnostics.office.com/#/) tööriista mõjutatud arvutis.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="b5ff7-104">Kui sõnum jääb teie väljundkaustas kinni, on kõige tõenäolisem põhjus suur manus või suvand "saada kohe, kui see on ühendatud" pole lubatud.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="b5ff7-105">**Eemaldage suur manus**</span><span class="sxs-lookup"><span data-stu-id="b5ff7-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="b5ff7-106">Klõpsake nuppu **Saada/võta vastu** > **Tööta ühenduseta**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b5ff7-107">Klõpsake navigeerimispaanil nuppu **Outbox**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="b5ff7-108">Siit saate:</span><span class="sxs-lookup"><span data-stu-id="b5ff7-108">From here, you can:</span></span> 
    - <span data-ttu-id="b5ff7-109">Kustutage sõnum.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-109">Delete the message.</span></span> <span data-ttu-id="b5ff7-110">Lihtsalt valige see ja klõpsake nuppu **Kustuta**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="b5ff7-111">Lohistage sõnum oma **mustandite kausta**, topeltklõpsake sõnumi avamiseks ja kustutage manus (klõpsake seda ja klõpsake nuppu **Kustuta**).</span><span class="sxs-lookup"><span data-stu-id="b5ff7-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="b5ff7-112">Kui tõrge ütleb, et Outlook proovib sõnumit edastada, sulgege Outlook.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b5ff7-113">Väljumiseks võib kuluda mõni hetk.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-113">It may take a few moments to exit.</span></span> <span data-ttu-id="b5ff7-114">Kui Outlook ei sulge, vajutage **klahvikombinatsiooni CTRL + ALT + DELETE** ja klõpsake nuppu **Käivita Tegumihaldur**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="b5ff7-115">Tegumihaldur, valige vahekaart **protsessid** , kerige Outlook. exe ja klõpsake **Lõpeta protsess**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="b5ff7-116">Pärast Outlook sulgub, taaskäivitage Outlook ja korrake samme 2-3.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="b5ff7-117">Pärast manuse eemaldamist klõpsake nuppu **Saada/võta vastu** > **ühenduseta** , et tühistada nupp ja jätkata tööd veebis.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="b5ff7-118">Sõnumid jäävad ka väljundkasti, kui klõpsate nuppu **saada**, kuid te ei ole ühendatud.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b5ff7-119">Klõpsake nuppu **Saada/võta vastu** ja vaadake **ühenduseta töö** nuppu.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b5ff7-120">Kui see on sinine, siis sa oled lahutatud.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b5ff7-121">Klõpsake seda ühendamiseks (nupp muutub valgeks) ja klõpsake **saada kõik**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b5ff7-122">**Luba saatmine kohe, kui see on ühendatud**</span><span class="sxs-lookup"><span data-stu-id="b5ff7-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="b5ff7-123">Klõpsake menüü Fail käsku **Suvandid**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="b5ff7-124">Klõpsake dialoogiboksis Outlooki suvandid nuppu **Täpsemalt**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="b5ff7-125">Klõpsake jaotises saatmise ja vastuvõtu lubamiseks **Saada kohe, kui**see on ühendatud.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="b5ff7-126">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="b5ff7-126">Click **OK**.</span></span>
 
<span data-ttu-id="b5ff7-127">Täielikud üksikasjad leiate teemast:</span><span class="sxs-lookup"><span data-stu-id="b5ff7-127">For full details, see:</span></span>
- [<span data-ttu-id="b5ff7-128">Video: saata või kustutada ummikus e-posti</span><span class="sxs-lookup"><span data-stu-id="b5ff7-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b5ff7-129">E-posti jääb kausta saatmiseks kuni te käsitsi algatada saatmise/vastuvõtu toiming Outlookis</span><span class="sxs-lookup"><span data-stu-id="b5ff7-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
