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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891745"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="e1d64-102">Outlook ei saa ühiskaustadega ühendust luua</span><span class="sxs-lookup"><span data-stu-id="e1d64-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="e1d64-103">Kui ühiskausta juurdepääs ei tööta mõned kasutajad, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="e1d64-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="e1d64-104">Ühendage EXO PowerShelli ja konfigureerige DefaultPublicFolderMailbox parameeter probleemi kasutajakonto sobitada parameeter töö kasutajakonto.</span><span class="sxs-lookup"><span data-stu-id="e1d64-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="e1d64-105">Näide:</span><span class="sxs-lookup"><span data-stu-id="e1d64-105">Example:</span></span>

<span data-ttu-id="e1d64-106">Get-postkasti WorkingUser | FT DefaultPublicFolderMailbox, Efektivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="e1d64-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="e1d64-107">Set-postkasti ProblemUser-DefaultPublicFolderMailbox \<väärtus eelmise käsu></span><span class="sxs-lookup"><span data-stu-id="e1d64-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="e1d64-108">Muudatuse jõustumiseks oodake vähemalt üks tund.</span><span class="sxs-lookup"><span data-stu-id="e1d64-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="e1d64-109">Kui probleem ei ole, Palun järgige [seda toimingut](https://aka.ms/pfcte) ühiskausta juurdepääsu probleemide tõrkeotsinguks Outlooki abil.</span><span class="sxs-lookup"><span data-stu-id="e1d64-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>