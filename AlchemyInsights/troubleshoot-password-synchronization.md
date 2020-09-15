---
title: Parooli sünkroonimise tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664922"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="61a25-102">Parooli sünkroonimise tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="61a25-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="61a25-103">Parooli sünkroonimise probleemide tõrkeotsinguks käivitage see AAD Connecti tõrkeotsing, et kindlaks teha, miks paroolid ei sünkroonita.</span><span class="sxs-lookup"><span data-stu-id="61a25-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="61a25-104">Alustuseks valige [Halda otsest sünkroonimist](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="61a25-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="61a25-105">Avage uus Windows PowerShelli seanss Azure AD Connecti serveris ja valige suvand **Käivita administraatorina** .</span><span class="sxs-lookup"><span data-stu-id="61a25-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="61a25-106">Run Set-ExecutionPolicy RemoteSigned või Set-ExecutionPolicy on piiramatud.</span><span class="sxs-lookup"><span data-stu-id="61a25-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="61a25-107">Käivitage Azure AD Connecti viisard.</span><span class="sxs-lookup"><span data-stu-id="61a25-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="61a25-108">Avage leht täiendavad tööülesanded > **tõrkeotsing**  >  **järgmiseks**.</span><span class="sxs-lookup"><span data-stu-id="61a25-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="61a25-109">Valige käsk **Käivita** , et avada menüü PowerShell tõrkeotsing.</span><span class="sxs-lookup"><span data-stu-id="61a25-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="61a25-110">Valige **parooli sünkroonimise tõrkeotsing**.</span><span class="sxs-lookup"><span data-stu-id="61a25-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="61a25-111">Probleem on tavaliselt selles, et parooli ei sünkroonita kindla kasutajakonto jaoks.</span><span class="sxs-lookup"><span data-stu-id="61a25-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="61a25-112">**Märkmed** Parooli sünkroonimine nurjub, kui viimase eduka parooli sünkroonimine oli mõni aeg tagasi.</span><span class="sxs-lookup"><span data-stu-id="61a25-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="61a25-113">Lisateavet parooli sünkroonimise tõrkeotsingu kohta leiate teemast [AZURE ad Connecti sünkroonimine parooliga Hash Synci tõrkeotsing](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="61a25-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>