---
title: Seade ootel olekus
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677571"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="eefe0-102">Seade ootel olekus</span><span class="sxs-lookup"><span data-stu-id="eefe0-102">Device in pending state</span></span>

<span data-ttu-id="eefe0-103">**Eeltingimused**</span><span class="sxs-lookup"><span data-stu-id="eefe0-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="eefe0-104">Kui häälestate seadme registreerimisi esimest korda, veenduge, et olete üle vaadanud rakenduse [Azure Active Directory (AZURE ad) seadmete halduse tutvustuse](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , mis juhendab teid, kuidas hankida seadmeid Azure AD ' i kontrolli all.</span><span class="sxs-lookup"><span data-stu-id="eefe0-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="eefe0-105">Kui registreerite seadmeid Azure AD otse ja registreerite need Intune ' i, peate veenduma, et olete [konfigureerinud Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ' i ja lubama kõigepealt [litsentsimise](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="eefe0-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="eefe0-106">Veenduge, et teil on lubatud sooritada toiminguid Azure AD ' is ja kohapealses REKLAAMIs.</span><span class="sxs-lookup"><span data-stu-id="eefe0-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="eefe0-107">Ainult Azure AD globaalne administraator saab seadme registreerimiste sätteid hallata.</span><span class="sxs-lookup"><span data-stu-id="eefe0-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="eefe0-108">Kui häälestate automaatseid registreerimisi asutusesiseses Active Directorys, peate olema Active Directory ja AD FS-i administraator (kui see on olemas).</span><span class="sxs-lookup"><span data-stu-id="eefe0-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="eefe0-109">Hübriid-Azure AD liitumise registreerimise protsess eeldab, et seadmed on ettevõtte võrgus.</span><span class="sxs-lookup"><span data-stu-id="eefe0-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="eefe0-110">See toimib ka VPN-i kaudu, kuid selle jaoks on mõned piirangud.</span><span class="sxs-lookup"><span data-stu-id="eefe0-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="eefe0-111">Oleme kuulnud kliente, kes vajavad abi hübriid-Azure AD joini registreerimise protsessis serveri töö tingimustes.</span><span class="sxs-lookup"><span data-stu-id="eefe0-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="eefe0-112">**Pilvepõhise autentimise keskkond (Azure AD Password Hash Synci või läbitud autentimise abil)**</span><span class="sxs-lookup"><span data-stu-id="eefe0-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="eefe0-113">Seda registreerimis voog on tuntud ka kui "Sünkrooni Liitu".</span><span class="sxs-lookup"><span data-stu-id="eefe0-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="eefe0-114">Järgnevalt on toodud, mis juhtub registreerimise käigus.</span><span class="sxs-lookup"><span data-stu-id="eefe0-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="eefe0-115">Windows 10 avastab teenuse liitumispunkti (SCP) kirje, kui kasutaja logib seadmesse sisse.</span><span class="sxs-lookup"><span data-stu-id="eefe0-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="eefe0-116">Seade proovib kõigepealt rentniku teavet, mis on pärit kliendipoolse SCP-i registrist [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="eefe0-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="eefe0-117">Lisateavet leiate teemast [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="eefe0-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="eefe0-118">Kui see ei õnnestu, suhtleb seade kohapealse Active Directoryga, et saada SCP-ist teavet rentniku kohta.</span><span class="sxs-lookup"><span data-stu-id="eefe0-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="eefe0-119">SCP-i kinnitamiseks viidake sellele [dokumendile](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="eefe0-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="eefe0-120">Soovitame teha aktiivses kataloogis SCP ja kasutada ainult kliendipoolse SCP-i algseks kinnitamiseks.</span><span class="sxs-lookup"><span data-stu-id="eefe0-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="eefe0-121">Windows 10 proovib Azure AD-ga suhelda süsteemi kontekstis, et autentida ennast Azure AD vastu.</span><span class="sxs-lookup"><span data-stu-id="eefe0-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="eefe0-122">Saate kontrollida, kas seadmel on süsteemi konto kaudu juurdepääs Microsofti ressurssidele, kasutades funktsiooni [test Device registreerimine ühenduvuse skripti](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="eefe0-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="eefe0-123">Windows 10 genereerib iseallkirjastatud serdi ja talletab selle arvuti objekti all asutusesiseses Active Directorys.</span><span class="sxs-lookup"><span data-stu-id="eefe0-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="eefe0-124">See eeldab, et domeenikontroller on vaateväljas.</span><span class="sxs-lookup"><span data-stu-id="eefe0-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="eefe0-125">Seadme objekt, mis sisaldab serti, sünkroonitakse Azure AD-ga Azure AD Connecti kaudu.</span><span class="sxs-lookup"><span data-stu-id="eefe0-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="eefe0-126">Sünkroonimise tsükkel on vaikimisi iga 30 minuti järel, kuid sõltub Azure AD Connecti konfiguratsioonist.</span><span class="sxs-lookup"><span data-stu-id="eefe0-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="eefe0-127">Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="eefe0-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="eefe0-128">Praeguses etapis peaks teil olema võimalus vaadata teema seadet jaotises "**Ootel**" olekus Azure ' i portaalis Device Blade.</span><span class="sxs-lookup"><span data-stu-id="eefe0-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="eefe0-129">Järgmise kasutaja sisselogimise korral versioonile Windows 10 on registreerimine lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="eefe0-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="eefe0-130">Kui kasutate VPN-i ja väljalogimine/logimine lõpetab domeeni ühenduvuse, saate käivitada registreerimise käsitsi.</span><span class="sxs-lookup"><span data-stu-id="eefe0-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="eefe0-131">Selleks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="eefe0-131">To do that:</span></span>
    >
    > <span data-ttu-id="eefe0-132">Väljastage `dsregcmd /join` kohalikult administraatori viip või PSExec kaudu arvuti kaudu.</span><span class="sxs-lookup"><span data-stu-id="eefe0-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="eefe0-133">Näiteks: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="eefe0-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="eefe0-134">Azure Active Directory seadme registreerimisega seotud levinumate probleemide kohta leiate teavet teemast [seadmete KKK](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="eefe0-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
