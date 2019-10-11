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
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441302"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="927e8-102">Sõnumite parandamine, mis on väljundkaustas kinni</span><span class="sxs-lookup"><span data-stu-id="927e8-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="927e8-103">Soovitame alustada, käivitades stsenaariumi ["Mul on probleeme saatmine, vastuvõtmine või leidmine"](https://aka.ms/SaRA-OutlookSendReceive) [Microsofti toe ja taastamise abimees](https://diagnostics.office.com/#/) tööriista.</span><span class="sxs-lookup"><span data-stu-id="927e8-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="927e8-104">Kui sõnum jääb teie väljundkaustas kinni, on kõige tõenäolisem põhjus:</span><span class="sxs-lookup"><span data-stu-id="927e8-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="927e8-105">Suured manused.</span><span class="sxs-lookup"><span data-stu-id="927e8-105">Large attachments.</span></span>
- <span data-ttu-id="927e8-106">**Saada kohe, kui ühendatud** suvand pole lubatud.</span><span class="sxs-lookup"><span data-stu-id="927e8-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="927e8-107">Suurte manuste eemaldamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="927e8-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="927e8-108">Outlookis valige **saatmise/vastuvõtu** > **töö ühenduseta**.</span><span class="sxs-lookup"><span data-stu-id="927e8-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="927e8-109">Valige navigeerimispaanil suvand **Väljundboks**.</span><span class="sxs-lookup"><span data-stu-id="927e8-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="927e8-110">Siit saate:</span><span class="sxs-lookup"><span data-stu-id="927e8-110">From here, you can:</span></span> 
    - <span data-ttu-id="927e8-111">Kustutage sõnum (valige see ja seejärel valige **Kustuta**).</span><span class="sxs-lookup"><span data-stu-id="927e8-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="927e8-112">Lohistage sõnum mustandite kausta, topeltklõpsake selle avamiseks ja manuse eemaldamiseks valige see ja seejärel valige **Kustuta**).</span><span class="sxs-lookup"><span data-stu-id="927e8-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="927e8-113">Kui kuvatakse tõrketeade, mis ütleb, et Outlook proovib sõnumit edastada, sulgege Outlook.</span><span class="sxs-lookup"><span data-stu-id="927e8-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="927e8-114">Väljumiseks võib kuluda mõni hetk.</span><span class="sxs-lookup"><span data-stu-id="927e8-114">It may take a few moments to exit.</span></span> <span data-ttu-id="927e8-115">Kui Outlook ei sulge, vajutage klahvikombinatsiooni CTRL + ALT + DELETE ja valige **Käivita Tegumihaldur**.</span><span class="sxs-lookup"><span data-stu-id="927e8-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="927e8-116">Valige Tegumihalduris vahekaart **protsessid** , kerige allapoole Outlook. exe ja valige **Lõpeta protsess**.</span><span class="sxs-lookup"><span data-stu-id="927e8-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="927e8-117">Pärast Outlooki sulgemist taaskäivitage see ja korrake juhiseid 2 ja 3.</span><span class="sxs-lookup"><span data-stu-id="927e8-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="927e8-118">Pärast manuse eemaldamist klõpsake nuppu **Saada/võta vastu** > **Tööta ühenduseta** , et jätkata töötamist ühendusega.</span><span class="sxs-lookup"><span data-stu-id="927e8-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="927e8-119">Sõnumid jäävad ka väljundkasti, kui klõpsate nuppu **saada**, kuid te ei ole ühendatud.</span><span class="sxs-lookup"><span data-stu-id="927e8-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="927e8-120">Klõpsake nuppu **Saada/võta vastu** ja vaadake **ühenduseta töö** nuppu.</span><span class="sxs-lookup"><span data-stu-id="927e8-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="927e8-121">Kui see on sinine, siis sa oled lahutatud.</span><span class="sxs-lookup"><span data-stu-id="927e8-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="927e8-122">Valige see ühendamiseks (nupp muutub valgeks) ja klõpsake nuppu **saada kõik**.</span><span class="sxs-lookup"><span data-stu-id="927e8-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="927e8-123">Et lubada **saatmise kohe, kui**see on ühendatud:</span><span class="sxs-lookup"><span data-stu-id="927e8-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="927e8-124">Valige >  **Täpsemad** **Failisuvandid** > \*\*\*\*.</span><span class="sxs-lookup"><span data-stu-id="927e8-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="927e8-125">Jaotises **saatmise ja vastuvõtu** valige **Saada kohe, kui**see on ühendatud, ja seejärel valige **OK**.</span><span class="sxs-lookup"><span data-stu-id="927e8-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="927e8-126">Täielikud üksikasjad on järgmised:</span><span class="sxs-lookup"><span data-stu-id="927e8-126">For full details see:</span></span>
- [<span data-ttu-id="927e8-127">Video: saata või kustutada ummikus e-posti</span><span class="sxs-lookup"><span data-stu-id="927e8-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="927e8-128">E-posti jääb kausta saatmiseks kuni te käsitsi algatada saatmise/vastuvõtu toiming Outlookis</span><span class="sxs-lookup"><span data-stu-id="927e8-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
