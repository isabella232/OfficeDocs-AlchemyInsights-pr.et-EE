---
title: Omanik ei saa Outlooki kaudu alamkausta luua
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665714"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="4635e-102">Omanik ei saa Outlooki kaudu alamkausta luua</span><span class="sxs-lookup"><span data-stu-id="4635e-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="4635e-103">**On käimas probleem avalike kaustade omanikega, mis loovad Outlooki abil alamkaustad. Probleem lahendatakse varsti.**</span><span class="sxs-lookup"><span data-stu-id="4635e-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="4635e-104">Vahepeal kasutage ühte järgmistest lahendustest.</span><span class="sxs-lookup"><span data-stu-id="4635e-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="4635e-105">Rakenduse Outlook for MAC kasutamine alamkausta loomiseks kui probleem mõjutab ainult Outlooki töölaua Windowsi versiooni (kõik versioonid)</span><span class="sxs-lookup"><span data-stu-id="4635e-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="4635e-106">Administraator luua alamkaust, kasutades EKSO Shell või EAC</span><span class="sxs-lookup"><span data-stu-id="4635e-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="4635e-107">Kasutaja DefaultPublicFolderMailbox/EffectivePublicFolderMailbox muutmine teise postkasti, kui selle kausta sisu postkast on probleemi põhjustanud</span><span class="sxs-lookup"><span data-stu-id="4635e-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="4635e-108">*Set-postkast user1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="4635e-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="4635e-109">Oodake tund, taaskäivitage Outlooki klientrakendus</span><span class="sxs-lookup"><span data-stu-id="4635e-109">Wait for an hour, restart outlook client</span></span>