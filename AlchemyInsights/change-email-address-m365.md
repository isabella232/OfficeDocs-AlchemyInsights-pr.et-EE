---
title: Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819076"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="daf46-102">Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmine</span><span class="sxs-lookup"><span data-stu-id="daf46-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="daf46-103">Microsoft 365 rühma või Microsoft Teamsi meiliaadressi muutmiseks saate kasutada [Microsoft 365 halduskeskust](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="daf46-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="daf46-104">Selleks valige rühm ja seejärel @redigeeri meiliaadressi.</span><span class="sxs-lookup"><span data-stu-id="daf46-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="daf46-105">Microsoft 365 rühma või Teamsi peamise SMTP-aadressi muutmiseks saate kasutada ka järgmist EXO PowerShelli käsku:</span><span class="sxs-lookup"><span data-stu-id="daf46-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="daf46-106">Näide:</span><span class="sxs-lookup"><span data-stu-id="daf46-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
