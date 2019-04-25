---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390413"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="2a0b7-102">Parooli sünkroonimise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="2a0b7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="2a0b7-103">Tõrkeotsingu, kus puuduvad paroolid on sünkroonitud Azure AD ühenduse versioon 1.1.614.0 või uuem versioon:</span><span class="sxs-lookup"><span data-stu-id="2a0b7-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="2a0b7-104">Avage uus Windows PowerShelli seanss Azure AD ühenduse serveri suvandiga **Käivita administraatorina** .</span><span class="sxs-lookup"><span data-stu-id="2a0b7-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="2a0b7-105">Käivitage **Set-ExecutionPolicy RemoteSigned** või **Set-ExecutionPolicy piiramatu**.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="2a0b7-106">Azure AD ühenduse viisardit käivitada.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="2a0b7-107">Liikuge selle \*\* lisaülesandeid \*\* avamiseks valige \*\* tõrkeotsing \*\*, ja klõpsake nuppu **edasi**.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="2a0b7-108">Klõpsake lehel tõrkeotsing **käivitada tõrkeotsingu käivitamiseks** menüü PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="2a0b7-109">Peamenüüst valige **Parooli sünkroonimise tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="2a0b7-110">Alammenüü, valige **parool ei tööta üldse**.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="2a0b7-111">**Arusaamiseks tõrkeotsingu ülesanne**</span><span class="sxs-lookup"><span data-stu-id="2a0b7-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="2a0b7-112">Tõrkeotsingu toiming teeb järgmised kontrollid:</span><span class="sxs-lookup"><span data-stu-id="2a0b7-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="2a0b7-113">Kinnitab, et parooli sünkroonimise funktsiooni on lubatud Azure AD üürnikule.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="2a0b7-114">Kinnitab, et Azure AD ühenduse server ei ole lavastus režiimis.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="2a0b7-115">Jaoks iga olemasoleva asutusesisese Active Directory konnektor (mis vastab olemasolevaid Active Directory metsa):</span><span class="sxs-lookup"><span data-stu-id="2a0b7-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="2a0b7-116">Kinnitab, et parooli sünkroonimise funktsioon on lubatud.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="2a0b7-117">Otsib parooli sünkroonimise pulss sündmused Windowsi rakenduste sündmuste logisse.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="2a0b7-118">Iga Active Directory domeeni all asutusesisese Active Directory konnektor:</span><span class="sxs-lookup"><span data-stu-id="2a0b7-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="2a0b7-119">Kinnitab, et on kättesaadav Azure AD ühenduse server.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="2a0b7-120">Kinnitab, et Active Directory Domain Services (AD DS) kontosid, mida asutusesisese Active Directory konnektor on õige kasutajanimi, parool ja parooli sünkroonimine vajalikud õigused.</span><span class="sxs-lookup"><span data-stu-id="2a0b7-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="2a0b7-121">Rohkem tõrkeotsing parooli sünkroonimise kohta vaadake teemast [tõrkeotsing parooli sünkroonimine Azure AD ühenduse sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="2a0b7-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

