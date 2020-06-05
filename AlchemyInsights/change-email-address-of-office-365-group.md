---
title: Microsoft 365 rühma e-posti aadressi muutmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580653"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="c6ffb-102">Microsoft 365 rühma e-posti aadressi muutmine</span><span class="sxs-lookup"><span data-stu-id="c6ffb-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="c6ffb-103">Saate muuta Microsoft 365 rühma e-posti aadress admin Center abil.</span><span class="sxs-lookup"><span data-stu-id="c6ffb-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c6ffb-104">Valige lihtsalt rühm ja valige @edit e-posti aadress.</span><span class="sxs-lookup"><span data-stu-id="c6ffb-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c6ffb-105">Võite kasutada ka EXO PowerShelli käsu abil saate muuta Microsoft 365 rühma esmane SMTP-aadress:</span><span class="sxs-lookup"><span data-stu-id="c6ffb-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="c6ffb-106">Komplekt-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c6ffb-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c6ffb-107">Näide:</span><span class="sxs-lookup"><span data-stu-id="c6ffb-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
