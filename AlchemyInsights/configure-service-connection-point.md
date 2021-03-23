---
title: Teenuse liitumispunkti konfigureerimine (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035451"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="17d0e-102">Teenuse liitumispunkti konfigureerimine (SCP)</span><span class="sxs-lookup"><span data-stu-id="17d0e-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="17d0e-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="17d0e-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="17d0e-104">**Põhjus**: SCP-objekti ei saa lugeda ja Azure AD rentniku teabe hankimine</span><span class="sxs-lookup"><span data-stu-id="17d0e-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="17d0e-105">**Resolutsioon**: vaadake jaotist [teenuse liitumispunkti konfigureerimine](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="17d0e-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="17d0e-106">**Tegevuskava**</span><span class="sxs-lookup"><span data-stu-id="17d0e-106">**Action plan**</span></span>

- <span data-ttu-id="17d0e-107">Kontrollige, kas seadmele on manustatud rühmapoliitika objekti, mida on kontrollitud.</span><span class="sxs-lookup"><span data-stu-id="17d0e-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="17d0e-108">Veenduge, et rühmapoliitika GPO on loonud registrivõtmed.</span><span class="sxs-lookup"><span data-stu-id="17d0e-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="17d0e-109">Veenduge, et teil oleks oma kataloogi ID ja onmicrosoft domeeniga loodud kaks võtit.</span><span class="sxs-lookup"><span data-stu-id="17d0e-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="17d0e-110">**Kliendipoolse registrisätete konfigureerimine SCP**</span><span class="sxs-lookup"><span data-stu-id="17d0e-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="17d0e-111">Järgmise näite abil saate luua rühmapoliitika objekti (GPO), et juurutada registri säte, mis konfigureerib teie seadmete registris SCP-kirje.</span><span class="sxs-lookup"><span data-stu-id="17d0e-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="17d0e-112">Avage rühmapoliitika halduskonsooli ja looge oma domeenis uus GPO.</span><span class="sxs-lookup"><span data-stu-id="17d0e-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="17d0e-113">Sisestage oma vastloodud GPO nimi (nt ClientSideSCP).</span><span class="sxs-lookup"><span data-stu-id="17d0e-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="17d0e-114">Redigeerige rühmapoliitika objekti ja otsige üles järgmine tee: **Arvuti konfiguratsioon > eelistused > Windowsi sätted > Registry**.</span><span class="sxs-lookup"><span data-stu-id="17d0e-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="17d0e-115">Paremklõpsake **registrit** ja valige **Uus > registri üksus**.</span><span class="sxs-lookup"><span data-stu-id="17d0e-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="17d0e-116">Konfigureerige vahekaardil **Üldine järgmine teave** .</span><span class="sxs-lookup"><span data-stu-id="17d0e-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="17d0e-117">**Toiming**: värskendamine</span><span class="sxs-lookup"><span data-stu-id="17d0e-117">**Action**: Update</span></span>
    
- <span data-ttu-id="17d0e-118">**Taru**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="17d0e-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="17d0e-119">**Võtme tee**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="17d0e-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="17d0e-120">**Väärtuse nimi**: TenantId</span><span class="sxs-lookup"><span data-stu-id="17d0e-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="17d0e-121">**Väärtuse tüüp**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="17d0e-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="17d0e-122">**Value data**: Azure AD eksemplari GUID või kataloogi ID (selle väärtuse leiate **Azure ' i portaalist > azure Active Directory > atribuudid > kataloogi ID**)</span><span class="sxs-lookup"><span data-stu-id="17d0e-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="17d0e-123">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="17d0e-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="17d0e-124">Paremklõpsake **registrit** ja valige **Uus > registri üksus**.</span><span class="sxs-lookup"><span data-stu-id="17d0e-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="17d0e-125">Konfigureerige vahekaardil **Üldine järgmine teave** .</span><span class="sxs-lookup"><span data-stu-id="17d0e-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="17d0e-126">**Toiming**: värskendamine</span><span class="sxs-lookup"><span data-stu-id="17d0e-126">**Action**: Update</span></span>
    
- <span data-ttu-id="17d0e-127">**Taru**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="17d0e-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="17d0e-128">**Võtme tee**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="17d0e-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="17d0e-129">**Väärtuse nimi**: TenantName</span><span class="sxs-lookup"><span data-stu-id="17d0e-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="17d0e-130">**Väärtuse tüüp**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="17d0e-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="17d0e-131">**Value data**: teie kinnitatud domeeninimi, kui kasutate välise keskkonna (nt AD FS).</span><span class="sxs-lookup"><span data-stu-id="17d0e-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="17d0e-132">Teie kinnitatud domeeninimi või teie onmicrosoft.com domeeninimi (nt contoso. onmicrosoft). com, kui kasutate hallatavat keskkonda</span><span class="sxs-lookup"><span data-stu-id="17d0e-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="17d0e-133">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="17d0e-133">Click **OK**.</span></span>

7. <span data-ttu-id="17d0e-134">Äsja loodud GPO redaktori sulgemine.</span><span class="sxs-lookup"><span data-stu-id="17d0e-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="17d0e-135">Lingi vastloodud GPO-ga soovitud OU sisaldavale domeeniga liitunud arvutitele, mis kuuluvad teie kontrollitava levikuga elanikkonnale.</span><span class="sxs-lookup"><span data-stu-id="17d0e-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="17d0e-136">Lisateavet leiate teemast [hübriid-AZURE ad Joint-AZURE ad kontrollitud valideerimine | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) ja  [tõrkeotsing hübriid-Azure Active Directory liitunud seadmed | Microsoft docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="17d0e-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









