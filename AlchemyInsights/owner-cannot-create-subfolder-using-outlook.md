---
title: Omanik ei saa outlooki abil alamkausta luua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748905"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="e5a93-102">Omanik ei saa outlooki abil alamkausta luua</span><span class="sxs-lookup"><span data-stu-id="e5a93-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="e5a93-103">**Käimas on probleem ühiskaustade omanike loomine alamkaustad Outlooki abil. Küsimus lahendatakse varsti.**</span><span class="sxs-lookup"><span data-stu-id="e5a93-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="e5a93-104">Vahepeal kasutage ühte järgmistest lahendused:</span><span class="sxs-lookup"><span data-stu-id="e5a93-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="e5a93-105">Kasutage Outlooki mac-i alamkausta loomiseks, kuna probleem mõjutab ainult Outlooki töölauaakende jaoks (kõik versioonid)</span><span class="sxs-lookup"><span data-stu-id="e5a93-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="e5a93-106">Kas admin luua alamkausta kasutades EXO Shell või EAC</span><span class="sxs-lookup"><span data-stu-id="e5a93-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="e5a93-107">Muutke DefaultPublicFolderMailbox/EffectivePublicFolderMailbox kasutaja muu postkasti kui sisu postkasti probleemi põhjustava kausta</span><span class="sxs-lookup"><span data-stu-id="e5a93-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="e5a93-108">*Set-postkasti kasutaja1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="e5a93-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="e5a93-109">Oodake tund, taaskäivitage Outlooki klient</span><span class="sxs-lookup"><span data-stu-id="e5a93-109">Wait for an hour, restart outlook client</span></span>