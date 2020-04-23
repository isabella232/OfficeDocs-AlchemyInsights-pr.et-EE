---
title: 1336 RecoverableItems kausta on täis
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720248"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="cd728-102">Kausta Taastatavad üksused on täis</span><span class="sxs-lookup"><span data-stu-id="cd728-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="cd728-103">Exchange Online ' i postkasti vaikimisi ladustamise piirang kausta Taastatavad üksused on 30 GB.</span><span class="sxs-lookup"><span data-stu-id="cd728-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="cd728-104">Taastatav üksuste kausta talletuslimiit suurendatakse automaatselt 100 GB-ga, kui postkast pannakse kohtuprotsessi Hold, eDiscovery ootel või on määratud säilituspoliitika.</span><span class="sxs-lookup"><span data-stu-id="cd728-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="cd728-105">Kui Taastatavad üksused kausta jõuab ladustamise piirang, postkasti funktsionaalsust mõjutab järgmistel viisidel:</span><span class="sxs-lookup"><span data-stu-id="cd728-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="cd728-106">Kasutaja ei saa kustutada üksusi postkasti.</span><span class="sxs-lookup"><span data-stu-id="cd728-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="cd728-107">Hallatav Kaustaabimees ei saa kustutada üksusi, mis põhinevad säilitusmärgil või hallatud kaustasätel.</span><span class="sxs-lookup"><span data-stu-id="cd728-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="cd728-108">Postkastid, mis on ühe üksuse taastamine lubatud või on paigutatud, Copy-on-kirjutada lehe kaitse protsess ei saa hallata kasutaja redigeeritud üksuste versioonid.</span><span class="sxs-lookup"><span data-stu-id="cd728-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="cd728-109">Postkastid, mis on postkasti auditilogi logimise lubatud, ei saa salvestada postkasti audit Logi kirjeid kausta Taastatavad üksused audit alamkausta.</span><span class="sxs-lookup"><span data-stu-id="cd728-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="cd728-110">Postkastid, mis ei ole kinni, administraatoritel saate kasutada `Search-Mailbox -SearchDumpsterOnly -DeleteContent` käsku Exchange Online PowerShelli üksuste kustutamiseks kausta Taastatavad üksused.</span><span class="sxs-lookup"><span data-stu-id="cd728-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="cd728-111">Lisateavet vaadake järgmistest teemadest:</span><span class="sxs-lookup"><span data-stu-id="cd728-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="cd728-112">Sõnumite otsimine ja kustutamine</span><span class="sxs-lookup"><span data-stu-id="cd728-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="cd728-113">Otsing-postkast</span><span class="sxs-lookup"><span data-stu-id="cd728-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="cd728-114">Postkastid, mis on hoida, administraatoritel eemaldada hoidke enne, kui nad saavad kustutatud üksuste kaustast Taastatavad üksused.</span><span class="sxs-lookup"><span data-stu-id="cd728-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="cd728-115">Lisateabe saamiseks vaadake [kustutage üksused pilvepõhiste postkastide kausta Taastatavad üksused hoida](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cd728-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="cd728-116">Et vältida Taastatavad üksused kausta saada täis, administraatoritel võib suurendada ladustamise piirang Taastatavad üksused kausta postkastid hoidke ja seadistada postkasti säilituspoliitika, mis teisaldab üksused kausta Taastatavad üksused kasutaja arhiivi postkasti.</span><span class="sxs-lookup"><span data-stu-id="cd728-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="cd728-117">Vaadake [suurendada Taastatavad üksused kvoodi postkasti hoida](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cd728-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
