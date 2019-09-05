---
title: Luba postkasti auditeerimine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736249"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="4022d-102">Luba postkasti auditeerimine</span><span class="sxs-lookup"><span data-stu-id="4022d-102">Enable mailbox auditing</span></span>

<span data-ttu-id="4022d-103">Postkasti auditeerimine lubamiseks kas ühe kasutaja või kogu organisatsiooni järgmised cmdlet-käsud tuleb käivitada kaugtöölaua Power Shell:</span><span class="sxs-lookup"><span data-stu-id="4022d-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="4022d-104">**Üksik kasutaja**</span><span class="sxs-lookup"><span data-stu-id="4022d-104">**Single User**</span></span>
  
<span data-ttu-id="4022d-105">Set-Mailbox-identiteedi "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="4022d-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="4022d-106">**Organisatsiooni**</span><span class="sxs-lookup"><span data-stu-id="4022d-106">**Organization**</span></span>
  
<span data-ttu-id="4022d-107">Get-Mailbox-ResultSize piiramatu-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="4022d-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="4022d-108">Lisateave</span><span class="sxs-lookup"><span data-stu-id="4022d-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

