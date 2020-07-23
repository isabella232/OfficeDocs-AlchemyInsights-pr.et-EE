---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387873"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="53186-102">Parooli sünkroonimise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="53186-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="53186-103">Parooli sünkroonimise probleemide tõrkeotsingu ks alustage selle AAD connect i tõrkeotsingu toimingu abil, et teha kindlaks, miks paroolid ei sünkroonita.</span><span class="sxs-lookup"><span data-stu-id="53186-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="53186-104">Alustamiseks [halda otsesünkroonimist](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="53186-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="53186-105">Avage uus Windows PowerShelli seanss oma Azure AD Ühenduse serveris ja valige suvand **Käivita administraatorina** .</span><span class="sxs-lookup"><span data-stu-id="53186-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="53186-106">Käivitage Set-ExecutionPolicy RemoteSigned või Set-ExecutionPolicy piiranguteta.</span><span class="sxs-lookup"><span data-stu-id="53186-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="53186-107">Käivitage Azure AD ühenduse viisard.</span><span class="sxs-lookup"><span data-stu-id="53186-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="53186-108">lehele Täiendavad tööülesanded > **Järgmine tõrkeotsing**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="53186-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="53186-109">PowerShelli tõrkeotsingumenüü avamiseks valige **Käivita.**</span><span class="sxs-lookup"><span data-stu-id="53186-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="53186-110">Valige **Parooli sünkroonimise tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="53186-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="53186-111">Probleem on tavaliselt selles, et parooli ei sünkroonita kindla kasutajakonto jaoks.</span><span class="sxs-lookup"><span data-stu-id="53186-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="53186-112">**Märkmed** Parooli sünkroonimine nurjub, kui viimane edukas parooli sünkroonimine oli mõni aeg tagasi.</span><span class="sxs-lookup"><span data-stu-id="53186-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="53186-113">Lisateavet parooli sünkroonimise tõrkeotsingu kohta leiate teemast [Parooli räsisünkroonimise tõrkeotsing Azure AD Connecti sünkroonimisega](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="53186-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>