---
title: Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798545"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="9a040-102">Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine</span><span class="sxs-lookup"><span data-stu-id="9a040-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="9a040-103">Microsoft 365 vastavuskeskuse uute ja täiustatud e-juurdluse funktsioonide tõttu lõpetatakse järgmiste kuude jooksul järgmised e-juurdluse tööriistad ja käsud.</span><span class="sxs-lookup"><span data-stu-id="9a040-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="9a040-104">[Exchange'i halduskeskuses on](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [olemas e-juurdlus](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) ja kohtne ootel.</span><span class="sxs-lookup"><span data-stu-id="9a040-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="9a040-105">Exchange Online'i PowerShelli cmdlet-käsud, mis In-Place e-juurdlust ja In-Place holds.</span><span class="sxs-lookup"><span data-stu-id="9a040-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="9a040-106">(Need cmdlet-käsud tuvastatakse ühiselt kui \*-MailboxSearchi cmdlet-käsud.) See hõlmab järgmisi cmdlet-käske.</span><span class="sxs-lookup"><span data-stu-id="9a040-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="9a040-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9a040-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="9a040-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9a040-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="9a040-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9a040-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="9a040-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="9a040-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="9a040-111">Exchange Online'i PowerShelli [cmdlet-käsk Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) (Otsingupostkast).</span><span class="sxs-lookup"><span data-stu-id="9a040-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="9a040-112">Exchange'i veebiteenuste API-s on järgmised toimingud.</span><span class="sxs-lookup"><span data-stu-id="9a040-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="9a040-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9a040-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="9a040-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9a040-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="9a040-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9a040-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="9a040-116">Täpsem e-juurdlus v1.0</span><span class="sxs-lookup"><span data-stu-id="9a040-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="9a040-117">**Pensionile jäämise ajaskaala:**</span><span class="sxs-lookup"><span data-stu-id="9a040-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="9a040-118">**1. juuli 2020** Te ei saa enam uusi otsinguid ja ootel otsimine, kuid saate olemasolevaid otsinguid ise käivitada, redigeerida ja kustutada.</span><span class="sxs-lookup"><span data-stu-id="9a040-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="9a040-119">Microsofti tugiteenused ei toeta enam In-Place e-juurdluse & EAC-s ootel.</span><span class="sxs-lookup"><span data-stu-id="9a040-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="9a040-120">**1. oktoobril 2020** In-Place E-juurdluse & EAC-s on ootel funktsioonid kirjutuskaitstud, nii et saate eemaldada ainult olemasolevad otsingud ja ootele pandud otsingud.</span><span class="sxs-lookup"><span data-stu-id="9a040-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="9a040-121">**Lisateavet leiate teemast**</span><span class="sxs-lookup"><span data-stu-id="9a040-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="9a040-122">E-juurdluse pärandotsingute ja -salvestatud üksuste migreerimine Microsoft 365 vastavuskeskusesse</span><span class="sxs-lookup"><span data-stu-id="9a040-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="9a040-123">Vanade e-juurdluse tööriistade kasutuselt kõrvaldamine</span><span class="sxs-lookup"><span data-stu-id="9a040-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="9a040-124">KKK e-juurdluse In-Place ja In-Place kohta</span><span class="sxs-lookup"><span data-stu-id="9a040-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



