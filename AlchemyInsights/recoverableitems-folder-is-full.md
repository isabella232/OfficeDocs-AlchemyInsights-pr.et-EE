---
title: 1336 RecoverableItems kaust on täis
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741263"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="8d7f0-102">Kaust Taastatavad üksused on täis</span><span class="sxs-lookup"><span data-stu-id="8d7f0-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="8d7f0-103">Exchange Online ' i postkastide jaoks on kausta Taastatavad üksused vaikeväärtuseks 30 GB.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="8d7f0-104">Kausta Taastatavad üksused salvestusruumi limiiti suurendatakse automaatselt 100 GB-ni, kui postkast paigutatakse ootele, e-juurdluse ootele või määratakse säilituspoliitika.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="8d7f0-105">Kui kaust Taastatavad üksused jõuab salvestusruumi piirmäärani, mõjutab see postkasti funktsioone järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="8d7f0-106">Kasutaja ei saa postkastist üksusi kustutada.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="8d7f0-107">Hallatava kausta assistent ei saa üksusi säilitus-või hallatava kausta sätete põhjal kustutada.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="8d7f0-108">Kui postkastid, millel on ühe üksuse taastamine lubatud või on paigutatud ootele, ei saa koopiat kirjutamise lehel säilitada kasutaja poolt redigeeritud üksuste versioone.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="8d7f0-109">Postkastide korral, millel on lubatud postkast audit, ei saa Postkasti auditilogi kirjeid salvestada kausta Taastatavad üksused.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="8d7f0-110">Kui postkastid pole ootel, saavad administraatorid kasutada `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShelli käsku, et kustutada üksused kaustas Taastatavad üksused.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="8d7f0-111">Lisateavet vaadake järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="8d7f0-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="8d7f0-112">Sõnumite otsimine ja kustutamine</span><span class="sxs-lookup"><span data-stu-id="8d7f0-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="8d7f0-113">Otsing – postkast</span><span class="sxs-lookup"><span data-stu-id="8d7f0-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="8d7f0-114">Postkastid, mis on ootel, peavad administraatorid eemaldama ootelepaneku, enne kui nad saavad üksused kaustast Taastatavad üksused kustutada.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="8d7f0-115">Lisateavet leiate teemast [pilvepõhise postkasti taastatavate üksuste kaustas olevate üksuste kustutamine ootel](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="8d7f0-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="8d7f0-116">Kui soovite, et kausta Taastatavad üksused ei muutuks täielikuks, võivad administraatorid ootel olevate postkastide kausta taastatavate üksuste salvestusruumi suurendada ja häälestada postkasti säilituspoliitika, mis teisaldab üksused kaustast Taastatavad üksused kasutaja arhiivi postkasti.</span><span class="sxs-lookup"><span data-stu-id="8d7f0-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="8d7f0-117">Vaadake teemat [postkasti taastatavate üksuste kvoodi suurendamine ootele](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="8d7f0-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
