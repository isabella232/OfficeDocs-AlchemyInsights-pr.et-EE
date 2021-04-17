---
title: Omanik ei saa Outlooki abil alamkausta luua
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836131"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="3e600-102">Omanik ei saa Outlooki abil alamkausta luua</span><span class="sxs-lookup"><span data-stu-id="3e600-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="3e600-103">**Avaliku kausta omanikel on käimas probleem alamkaustade loomisega Outlooki abil. Probleem lahendatakse peagi.**</span><span class="sxs-lookup"><span data-stu-id="3e600-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="3e600-104">Samal ajal kasutage ühte järgmistest lahendustest.</span><span class="sxs-lookup"><span data-stu-id="3e600-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="3e600-105">Outlook for MAC-i abil alamkausta loomine, kuna probleem mõjutab ainult Outlooki töölauaaknaid (kõiki versioone)</span><span class="sxs-lookup"><span data-stu-id="3e600-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="3e600-106">Kas administraator loob alamkausta EXO Shelli või EAC abil</span><span class="sxs-lookup"><span data-stu-id="3e600-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="3e600-107">Muutke kasutaja defaultPublicFolderMailbox/EffectivePublicFolderMailboxiks muuks postkastiks kui kausta sisupostkast, mis põhjustab probleemi</span><span class="sxs-lookup"><span data-stu-id="3e600-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="3e600-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="3e600-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="3e600-109">Oodake tund, taaskäivitage Outlooki klientrakendus</span><span class="sxs-lookup"><span data-stu-id="3e600-109">Wait for an hour, restart outlook client</span></span>