---
title: CompletedWithErrors olekuga ühiskausta migreerimise pakett
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744109"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="250a6-102">CompletedWithErrors olekuga ühiskausta migreerimise pakett</span><span class="sxs-lookup"><span data-stu-id="250a6-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="250a6-103">Tehke paketti viimiseks järgmised toimingud, jättes vahele suured/halvad üksused.</span><span class="sxs-lookup"><span data-stu-id="250a6-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="250a6-104">Siirdamispartii vahele jäetud üksuste kinnitamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="250a6-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="250a6-105">Kasutage järgmist käsku, et kinnitada migreerimise päringute vahele jäetud üksused, mis on sünkroonitud, kuid pole lõpule viidud.</span><span class="sxs-lookup"><span data-stu-id="250a6-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="250a6-106">Migreerimise pakett ja taotlused tuleks mõne minuti pärast uuesti alustada ja täita.</span><span class="sxs-lookup"><span data-stu-id="250a6-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

