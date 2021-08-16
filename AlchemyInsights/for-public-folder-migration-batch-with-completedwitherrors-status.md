---
title: Avaliku kausta migreerimispaketi jaoks, mille olek on CompletedWithErrors
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
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068160"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Avaliku kausta migreerimispaketi jaoks, mille olek on CompletedWithErrors

Paketi lõpuleviimiseks tehke järgmist. Suurte/halbade üksuste vahelejätmiseks tehke järgmist. 
1. Migreerimispaketi vahelejäetud üksuste kinnitamine

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Järgmise käsu abil saate kinnitada vahelejäetud üksused migreerimistaotlustes, mis on "Sünkroonitud", kuid mida pole lõpule viidud.

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Migreerimispaketi ja -päringute jätkumine ja lõpule viimine peaks mõne minuti pärast jätkuma.

