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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282710"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="a39e1-102">Microsoft 365 rühma e-posti aadressi muutmine</span><span class="sxs-lookup"><span data-stu-id="a39e1-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="a39e1-103">Saate muuta Microsoft 365 rühma e-posti aadress admin Center abil.</span><span class="sxs-lookup"><span data-stu-id="a39e1-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="a39e1-104">Valige lihtsalt rühm ja valige @edit e-posti aadress.</span><span class="sxs-lookup"><span data-stu-id="a39e1-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="a39e1-105">Võite kasutada ka EXO PowerShelli käsu abil saate muuta Microsoft 365 rühma esmane SMTP-aadress:</span><span class="sxs-lookup"><span data-stu-id="a39e1-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="a39e1-106">Komplekt-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="a39e1-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="a39e1-107">Näide:</span><span class="sxs-lookup"><span data-stu-id="a39e1-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
