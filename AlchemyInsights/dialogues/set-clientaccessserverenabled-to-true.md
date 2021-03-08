---
title: ClientAccessServerEnabled seadmine True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524559"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="bce7e-102">ClientAccessServerEnabled seadmine True</span><span class="sxs-lookup"><span data-stu-id="bce7e-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="bce7e-103">Kui te ei saa krüptitud meilisõnumit avada ja selle asemel vaadata **rpmsg** manust, tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="bce7e-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="bce7e-104">Ühenduse loomine Exchange Online PowerShelliga.</span><span class="sxs-lookup"><span data-stu-id="bce7e-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="bce7e-105">Exchange Online PowerShelliga ühenduse loomiseks peate sisse logima üldise administraatori või Exchange ' i administraatori konto abil.</span><span class="sxs-lookup"><span data-stu-id="bce7e-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="bce7e-106">loomine.</span><span class="sxs-lookup"><span data-stu-id="bce7e-106">a.</span></span> <span data-ttu-id="bce7e-107">Avage Windows PowerShell ja käivitage järgmine käsk. `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="bce7e-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="bce7e-108">b.</span><span class="sxs-lookup"><span data-stu-id="bce7e-108">b.</span></span> <span data-ttu-id="bce7e-109">Sisestage dialoogiboksis **Windows PowerShelli mandaadi taotlus** oma töö-või kooli konto ja parool, c.</span><span class="sxs-lookup"><span data-stu-id="bce7e-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="bce7e-110">Klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="bce7e-110">Click **OK**.</span></span> 

2. <span data-ttu-id="bce7e-111">Uue seansi loomiseks käivitage järgmine käsk.</span><span class="sxs-lookup"><span data-stu-id="bce7e-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="bce7e-112">loomine.</span><span class="sxs-lookup"><span data-stu-id="bce7e-112">a.</span></span> <span data-ttu-id="bce7e-113">Käivitage järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="bce7e-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="bce7e-114">`Get-IRMConfiguration`Käsk Käivita.</span><span class="sxs-lookup"><span data-stu-id="bce7e-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="bce7e-115">Märkige **ClientAccessServerEnabled** säte.</span><span class="sxs-lookup"><span data-stu-id="bce7e-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="bce7e-116">loomine.</span><span class="sxs-lookup"><span data-stu-id="bce7e-116">a.</span></span> <span data-ttu-id="bce7e-117">Kui **ClientAccessServerEnabled** säte on seatud väärtusele **FALSE**, käivitage järgmine cmdlet-käsk. `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="bce7e-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="bce7e-118">Sulgege oma PowerShelli seanss alati järgmise käsuga: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="bce7e-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="bce7e-119">Lisateavet leiate teemast [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="bce7e-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

