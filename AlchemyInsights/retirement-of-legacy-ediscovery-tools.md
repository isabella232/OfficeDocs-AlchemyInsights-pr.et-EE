---
title: Pärand eDiscovery tööriistade pensionile jäämine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600361"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="3686f-102">Pärand eDiscovery tööriistade pensionile jäämine</span><span class="sxs-lookup"><span data-stu-id="3686f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="3686f-103">Uue ja täiustatud eDiscovery funktsiooni Microsoft 365 vastavuse Center tulemusena on järgmised pärand eDiscovery tööriistad ja commandlette lähikuudel pensionile:</span><span class="sxs-lookup"><span data-stu-id="3686f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="3686f-104">Kohapealse [eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) ja kohapealse [hoiab](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange ' i halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="3686f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="3686f-105">Exchange Online PowerShelli cmdlet-käsud, mis toetavad kohapealse eDiscovery ja kohapealse hoiab.</span><span class="sxs-lookup"><span data-stu-id="3686f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="3686f-106">(Need cmdlet-käsud on ühiselt määratletud kui \*-MailboxSearch cmdlet-käsud.) See hõlmab järgmisi cmdlet-käske:</span><span class="sxs-lookup"><span data-stu-id="3686f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="3686f-107">Uus MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3686f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="3686f-108">Alusta-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3686f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="3686f-109">Stopp-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3686f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="3686f-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3686f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="3686f-111">[Otsing postkasti cmdlet-](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) käsu Exchange Online PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="3686f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="3686f-112">Järgmised toimingud Exchange ' i veebiteenuste API-s:</span><span class="sxs-lookup"><span data-stu-id="3686f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="3686f-113">Getsearchablepostkastid</span><span class="sxs-lookup"><span data-stu-id="3686f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="3686f-114">Setholdonpostkastid</span><span class="sxs-lookup"><span data-stu-id="3686f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="3686f-115">Getholdonpostkastid</span><span class="sxs-lookup"><span data-stu-id="3686f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="3686f-116">Office 365 täpsem eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="3686f-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="3686f-117">**Pensionile jäämise ajakava**:</span><span class="sxs-lookup"><span data-stu-id="3686f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="3686f-118">1. aprill 2020: te ei saa luua uusi otsinguid ja hoiab, kuid saate endiselt käivitada, redigeerida ja kustutada olemasolevaid otsinguid omal vastutusel.</span><span class="sxs-lookup"><span data-stu-id="3686f-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="3686f-119">Microsoft support ei toeta enam kohapealse eDiscovery & hoiab EAC.</span><span class="sxs-lookup"><span data-stu-id="3686f-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="3686f-120">1. juuli 2020: kohapealse eDiscovery & hoiab funktsiooni EAC paigutatakse kirjutuskaitstud režiimis.</span><span class="sxs-lookup"><span data-stu-id="3686f-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="3686f-121">See tähendab, et teil on võimalik eemaldada ainult olemasolevad otsingud ja hoidmised.</span><span class="sxs-lookup"><span data-stu-id="3686f-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="3686f-122">**Lisateabe saamiseks vaadake**:</span><span class="sxs-lookup"><span data-stu-id="3686f-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="3686f-123">Migreerimine pärand eDiscovery otsingud ja hoiab Microsoft 365 vastavuse keskus</span><span class="sxs-lookup"><span data-stu-id="3686f-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="3686f-124">Pärand eDiscovery tööriistade pensionile jäämine</span><span class="sxs-lookup"><span data-stu-id="3686f-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="3686f-125">KKK kohapealse eDiscovery ja kohapealse valda kohta</span><span class="sxs-lookup"><span data-stu-id="3686f-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



