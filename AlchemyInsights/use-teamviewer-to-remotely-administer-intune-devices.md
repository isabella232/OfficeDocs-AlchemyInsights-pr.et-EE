---
title: TeamViewer kasutamine Intune Devices kaugjuhtimiseks haldamiseks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554973"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="45d2d-102">TeamViewer kasutamine Intune Devices kaugjuhtimiseks haldamiseks</span><span class="sxs-lookup"><span data-stu-id="45d2d-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="45d2d-103">Intune ' i hallatavaid seadmeid saab [TeamViewer](https://www.teamviewer.com/)abil eemalt hallata.</span><span class="sxs-lookup"><span data-stu-id="45d2d-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="45d2d-104">Intune ' i haldamiseks funktsiooni TeamViewer abil tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="45d2d-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="45d2d-105">Alustuseks Hankige mandaat alates TeamViewer, et häälestada TeamViewer konnektor Intune.</span><span class="sxs-lookup"><span data-stu-id="45d2d-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="45d2d-106">See võimaldab administraatoril sisestada mandaate TeamViewer Connectori KASUTAJALIIDESE jaotises seadmed, ühekordne toiming, et luua link Intune ' i ja TeamViewer teenuse vahel.</span><span class="sxs-lookup"><span data-stu-id="45d2d-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="45d2d-107">**1. osa: seansi alustamine kaugarvutiga**</span><span class="sxs-lookup"><span data-stu-id="45d2d-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="45d2d-108">Valige jaotises **kõik seadmed**seade, millega soovite seansi alustada.</span><span class="sxs-lookup"><span data-stu-id="45d2d-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="45d2d-109">Alates \*\*... \*\*Valige **Uus Kaugabi seanss**.</span><span class="sxs-lookup"><span data-stu-id="45d2d-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="45d2d-110">Valige **Jah** , et kinnitada, et soovite luua seansi.</span><span class="sxs-lookup"><span data-stu-id="45d2d-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="45d2d-111">Pärast seda, kui TeamViewer teenus on kinnitanud taotluse "uue serveri seansi alustamine", kuvatakse teile suvand **kaugabi käivitamiseks** seadme ülevaate (või Essentialsi) üksikasjade alusel.</span><span class="sxs-lookup"><span data-stu-id="45d2d-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="45d2d-112">Paani laiendamiseks ja kaugabi oleku kuvamiseks valige Kuva **rohkem** .</span><span class="sxs-lookup"><span data-stu-id="45d2d-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="45d2d-113">Seansi alustamiseks administraatori poole valige **Käivita Kaugseanss** .</span><span class="sxs-lookup"><span data-stu-id="45d2d-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="45d2d-114">Valige TeamViewer binaarne (Windows) ja valige **Käivita**.</span><span class="sxs-lookup"><span data-stu-id="45d2d-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="45d2d-115">**Märkus** Saate ignoreerida mis tahes veebibrauseri lehte, mis on avatud TeamViewer veebisaidile.</span><span class="sxs-lookup"><span data-stu-id="45d2d-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="45d2d-116">Kinnitage rakenduse TeamViewer taotlus teha muudatusi seadmes (ainult Windowsis).</span><span class="sxs-lookup"><span data-stu-id="45d2d-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="45d2d-117">TeamViewer rakendus käivitub ja sisaldab seansi koodi, et autentida ühendust kaugserveri seadmega.</span><span class="sxs-lookup"><span data-stu-id="45d2d-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="45d2d-118">**Osa 2: seadmes, mis on suunatud serveri seansile**</span><span class="sxs-lookup"><span data-stu-id="45d2d-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="45d2d-119">Avage Intune ettevõtte portaal.</span><span class="sxs-lookup"><span data-stu-id="45d2d-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="45d2d-120">Teatise lipu otsimine: "teie IT-administraator palub selle seadme juhtelementi Kaugabi seansi jaoks" ja valige teatis.</span><span class="sxs-lookup"><span data-stu-id="45d2d-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="45d2d-121">Valige TeamViewer rakenduse allalaadimine või TeamViewer rakenduse allalaadimine App Store ' ist ja valige **Käivita**.</span><span class="sxs-lookup"><span data-stu-id="45d2d-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="45d2d-122">**Märkus** Saate ignoreerida mis tahes veebibrauseri lehte, mis on avatud TeamViewer veebisaidile.</span><span class="sxs-lookup"><span data-stu-id="45d2d-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="45d2d-123">Kinnitage rakenduse TeamViewer taotlus teha muudatusi seadmes (ainult Windowsis).</span><span class="sxs-lookup"><span data-stu-id="45d2d-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="45d2d-124">TeamViewer rakendus käivitub ja sisaldab seansi koodi, et autentida ühendust kaugserveri seadmega.</span><span class="sxs-lookup"><span data-stu-id="45d2d-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="45d2d-125">Hüpik küsib, kas soovite seansi avakuvale lubada.</span><span class="sxs-lookup"><span data-stu-id="45d2d-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="45d2d-126">**Märkus** TeamViewer teenus genereeritud seansi koodid on ainult ühekordseks kasutamiseks.</span><span class="sxs-lookup"><span data-stu-id="45d2d-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="45d2d-127">Kui kaotate ühendust, peate tegema järgmist.</span><span class="sxs-lookup"><span data-stu-id="45d2d-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="45d2d-128">Sulgege TeamViewer rakenduse eksemplar kaugarvutis ja administraatori tööjaamas.</span><span class="sxs-lookup"><span data-stu-id="45d2d-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="45d2d-129">Sulgege Kaug-seadmes ettevõtte portaal.</span><span class="sxs-lookup"><span data-stu-id="45d2d-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="45d2d-130">Alustage administraatori portaalist uut uut kaugabi seanssi.</span><span class="sxs-lookup"><span data-stu-id="45d2d-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="45d2d-131">Uue teatise vastuvõtmiseks avage serveri seadmes uuesti ettevõtte portaal.</span><span class="sxs-lookup"><span data-stu-id="45d2d-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="45d2d-132">Laadige alla ja avage TeamViewer rakendus nii kaugarvutis kui ka administraatori tööjaamas.</span><span class="sxs-lookup"><span data-stu-id="45d2d-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>