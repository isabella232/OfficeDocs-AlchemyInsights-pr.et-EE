---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732506"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="4d6c2-102">Parooli sünkroonimise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="4d6c2-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="4d6c2-103">Tõrkeotsing probleemidele, kus paroolid on sünkroonitud Azure AD ühenduse versiooni 1.1.614.0 või uuem versioon:</span><span class="sxs-lookup"><span data-stu-id="4d6c2-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="4d6c2-104">Avage uus Windows PowerShelli seansi Azure AD ühenduse serveris suvandi **Käivita administraatorina** .</span><span class="sxs-lookup"><span data-stu-id="4d6c2-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="4d6c2-105">Käivitage **Set-ExecutionPolicy Remoteallkirjastatud** või **seatud-ExecutionPolicy piiranguteta**.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="4d6c2-106">Käivitage Azure AD ühenduse viisard.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="4d6c2-107">Liikuge lehele **täiendavad tööülesanded** , valige **tõrkeotsing**ja klõpsake nuppu **edasi**.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="4d6c2-108">Klõpsake lehel tõrkeotsing **käivitada PowerShelli tõrkeotsingu menüü käivitamiseks** .</span><span class="sxs-lookup"><span data-stu-id="4d6c2-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="4d6c2-109">Valige põhimenüüs **parooli sünkroonimise tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="4d6c2-110">Alammenüüs valige **parooli sünkroonimine ei tööta üldse**.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="4d6c2-111">**Tõrkeotsinguülesande tulemuste mõistmine**</span><span class="sxs-lookup"><span data-stu-id="4d6c2-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="4d6c2-112">Tõrkeotsingu ülesanne teeb järgmised kontrollid:</span><span class="sxs-lookup"><span data-stu-id="4d6c2-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="4d6c2-113">Valideerib, et parooli sünkroonimise funktsioon on lubatud Azure AD rentniku jaoks.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="4d6c2-114">Valideerib Azure AD ühenduse server ei ole vahekausta režiimis.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="4d6c2-115">Iga olemasoleva asutusesisese Active Directory konnektor (mis vastab olemasolevale Active Directory metsa):</span><span class="sxs-lookup"><span data-stu-id="4d6c2-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="4d6c2-116">Valideerib, et parooli sünkroonimise funktsioon on lubatud.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="4d6c2-117">Otsib parooli sünkroonimise südamelöögi sündmused Windowsi rakenduse sündmuselogid.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="4d6c2-118">Iga Active Directory domeeni asutusesisese Active Directory konnektor:</span><span class="sxs-lookup"><span data-stu-id="4d6c2-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="4d6c2-119">Valideerib, et domeen on kättesaadav Azure AD ühenduse serverist.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="4d6c2-120">Valideerib, et Active Directory domeeniteenused (AD DS) kontod, mida kasutatakse asutusesisese Active Directory konnektor on õige kasutajanimi, parool ja õigused parooli sünkroonimine.</span><span class="sxs-lookup"><span data-stu-id="4d6c2-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="4d6c2-121">Parooli sünkroonimise tõrkeotsingu kohta lisateabe saamiseks vaadake [tõrkeotsing parooli sünkroonimine AZURE AD ühenduse sünkroonimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="4d6c2-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  