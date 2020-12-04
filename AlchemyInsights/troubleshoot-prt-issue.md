---
title: PRT probleemi tõrkeotsing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573494"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="4d3fe-102">PRT probleemi tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="4d3fe-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="4d3fe-103">Kui soovite autentimine uuesti sooritada, peab see olema täielikult registreeritud ja heas olekus ning hankima esmase värskendamise tõendi (PRT).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="4d3fe-104">Hübriid-Azure AD liitumise registreerimise protsess eeldab, et seadmed peavad olema ettevõtte võrgus.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="4d3fe-105">See toimib ka VPN-i kaudu, kuid selle jaoks on mõned piirangud.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="4d3fe-106">Oleme kuulnud kliente, kes vajavad abi seoses hübriid-Azure AD Jointi registreerimisega, mis on seotud Kaug-töö asjaoludega.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="4d3fe-107">Siin on jaotus, mis toimub "kapoti all" registreerimise käigus.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="4d3fe-108">**Pilvepõhise autentimise keskkond (Azure AD Password Hash Synci või läbitud autentimise abil)**</span><span class="sxs-lookup"><span data-stu-id="4d3fe-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="4d3fe-109">Seda registreerimis voog on tuntud ka kui "Sünkrooni Liitu".</span><span class="sxs-lookup"><span data-stu-id="4d3fe-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="4d3fe-110">Windows 10 avastas SCP-kirje kasutaja sisselogimise korral seadmesse.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="4d3fe-111">Seade proovib kõigepealt rentniku teavet, mis on pärit kliendipoolse SCP-i registrist [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="4d3fe-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="4d3fe-112">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="4d3fe-113">Kui see ei õnnestu, suhtleb seade kohapealse Active Directoryga (AD), et saada rentniku teavet teenusest Connection Point (SCP).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="4d3fe-114">SCP-i kontrollimiseks lugege seda [dokumenti](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="4d3fe-115">Soovitame anda REKLAAMIle SCP ja kasutada seda ainult kliendipoolse SCP-i esmaseks kinnitamiseks.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="4d3fe-116">Windows 10 proovib Azure AD-ga suhelda süsteemi kontekstis, et autentida ennast Azure AD vastu.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="4d3fe-117">Saate kontrollida, kas seadmel on süsteemi konto kaudu juurdepääs Microsofti ressurssidele, kasutades funktsiooni test Device registreerimine ühenduvuse skripti.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="4d3fe-118">Windows 10 loob iseallkirjastatud serdi ja salvestab selle kohapeal asuvas arvutis asuvale objektile.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="4d3fe-119">See eeldab, et domeenikontroller on vaateväljas.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="4d3fe-120">Seadme objekt, mis on serdi saab sünkroonida Azure AD kaudu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="4d3fe-121">Sünkroonimise tsükkel on vaikimisi iga 30 minuti järel, kuid sõltub Azure AD Connecti konfiguratsioonist.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="4d3fe-122">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="4d3fe-123">Praeguses etapis peaks teil olema võimalus vaadata teema seadet jaotises "ootel" olekus Azure ' i portaalis Device Blade.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="4d3fe-124">Järgmise kasutaja sisselogimise korral versioonile Windows 10 on registreerimine lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="4d3fe-125">Kui kasutate VPN-i ja väljalogimine – sisselogimise protsess katkestab domeeni ühenduvuse, saate käivitada registreerimise käsitsi.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="4d3fe-126">Väljastage dsregcmd/JOIN kohalikult administraatori viibale või PSExec kaudu teie ARVUTISSE.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="4d3fe-127">Näiteks PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="4d3fe-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="4d3fe-128">Lisateavet hübriidiga liitumise probleemide kohta leiate teemast [seadmete probleemi tõrkeotsing](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
