---
title: Ühiskaustadele ei pääse juurde
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
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959491"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a6622-102">Outlook ei saa ühiskaustadega ühendust luua</span><span class="sxs-lookup"><span data-stu-id="a6622-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a6622-103">Kui ühiskausta juurdepääs ei tööta vähe kasutajaid, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="a6622-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="a6622-104">Ühendage EXO PowerShelli ja konfigureerige DefaultPublicFolderMailbox probleemi kasutajakonto sobitada ühe töö kasutaja konto.</span><span class="sxs-lookup"><span data-stu-id="a6622-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="a6622-105">Näide:</span><span class="sxs-lookup"><span data-stu-id="a6622-105">Example:</span></span>

<span data-ttu-id="a6622-106">Get-postkasti WorkingUser | FT DefaultPublicFolderMailbox, Efektivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="a6622-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a6622-107">Set-postkasti ProblemUser-DefaultPublicFolderMailbox \<väärtus eelmise käsu></span><span class="sxs-lookup"><span data-stu-id="a6622-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a6622-108">Muudatuse jõustumiseks oodake vähemalt üks tund.</span><span class="sxs-lookup"><span data-stu-id="a6622-108">Wait at least one hour for the change to take effect.</span></span>