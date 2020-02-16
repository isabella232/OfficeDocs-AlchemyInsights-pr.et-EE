---
title: Ühiskausta migreerimise partii CompletedWithErrors olek
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043581"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Ühiskausta migreerimise partii CompletedWithErrors olek

Pakktöötluse lõpuleviimiseks, suurte/halbade üksuste vahelejätmine toimige järgmiselt. 
1. Kinnitage vahelejäetud üksused migreerimispaketi puhul:

    Set-Migrationpartii \<batchname>-ApproveSkippedItems 
2. Järgmise käsu abil saate kinnitada vahelejäetud üksused migratsiooni taotlusi, mis on "sünkroonitud", kuid ei ole lõpule viidud:

    $pf = Get-PublicFolderMailboxMigrationRequest | Hankige-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i $pf) {IF ($i. LargeItemsEncountered-gt 0-või $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. identiteedi. IdentifyingGuid-SkippedItemApprovalTime $ ([kuupäev kellaaeg]:: UtcNow)}}
3. Migreerimispaketi ja taotlused peaks uuesti ja lõpule mõne minuti.

