---
title: Legacy-e-juurdluse tööriistade kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727779"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="0f302-102">Legacy-e-juurdluse tööriistade kasutuselt kõrvaldamine</span><span class="sxs-lookup"><span data-stu-id="0f302-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="0f302-103">Microsoft 365 nõuetele vastavuse keskuses uute ja täiustatud e-juurdluse funktsioonide tulemusena aeguvad järgnevatel kuudel järgmised pärand e-juurdluse e-juurdluse tööriistad ja Commandlets.</span><span class="sxs-lookup"><span data-stu-id="0f302-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="0f302-104">Kohapealne e [-juurdlus](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ja kohapeal on Exchange](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) ' i halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="0f302-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="0f302-105">Exchange Online ' i PowerShelli cmdlet-käsud, mis toetavad kohapealset e-juurdlust ja kohapealset olemasolu.</span><span class="sxs-lookup"><span data-stu-id="0f302-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="0f302-106">(Need cmdlet-käsud määratakse ühiselt \*-MailboxSearch cmdlet-käskudeks.) See hõlmab järgmisi cmdlet-käske.</span><span class="sxs-lookup"><span data-stu-id="0f302-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="0f302-107">Uus-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0f302-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="0f302-108">Start – MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0f302-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="0f302-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0f302-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="0f302-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="0f302-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="0f302-111">Exchange Online ' i PowerShelli cmdlet [-käsk Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) .</span><span class="sxs-lookup"><span data-stu-id="0f302-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="0f302-112">Järgmised toimingud Exchange Web Services API-s:</span><span class="sxs-lookup"><span data-stu-id="0f302-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="0f302-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="0f302-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="0f302-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0f302-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="0f302-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="0f302-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="0f302-116">Täiustatud e-juurdlus v 1.0</span><span class="sxs-lookup"><span data-stu-id="0f302-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="0f302-117">**Pensionile jäämise ajakava**:</span><span class="sxs-lookup"><span data-stu-id="0f302-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="0f302-118">**1. juuli 2020** Uusi otsinguid ja ootelepaneku ei saa enam luua, kuid saate olemasolevaid otsinguid käivitada, redigeerida ja kustutada omal riisikol.</span><span class="sxs-lookup"><span data-stu-id="0f302-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="0f302-119">Microsoft support ei toeta enam kohapealset e-juurdlust & kuulub EAC-sse.</span><span class="sxs-lookup"><span data-stu-id="0f302-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="0f302-120">**1. oktoober 2020** Veebipõhine e-juurdlus & omab EAC-s funktsioone, mis kuvatakse kirjutuskaitstud režiimis, et saaksite eemaldada ainult olemasolevad otsingud ja ootelepanekud.</span><span class="sxs-lookup"><span data-stu-id="0f302-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="0f302-121">**Lisateavet leiate järgmistest teemadest**.</span><span class="sxs-lookup"><span data-stu-id="0f302-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="0f302-122">Pärandist e-juurdluse otsingute migreerimine ja Microsoft 365 nõuetele vastavuse keskus</span><span class="sxs-lookup"><span data-stu-id="0f302-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="0f302-123">Legacy-e-juurdluse tööriistade kasutuselt kõrvaldamine</span><span class="sxs-lookup"><span data-stu-id="0f302-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="0f302-124">KKK-kohapealne e-juurdlus ja kohapealne tööpõhimõte</span><span class="sxs-lookup"><span data-stu-id="0f302-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



