---
title: Meilisõnumite edastamine Microsoft 365 kaudu
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809651"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="63914-102">Mitmeotstarbelise seadme või rakenduse häälestamine meili saatma</span><span class="sxs-lookup"><span data-stu-id="63914-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="63914-103">Teavet variantide kohta ja juhised leiate artiklist [Mitmeotstarbelise seadme või rakenduse häälestamine Microsoft 365 kaudu meili saatma](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="63914-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="63914-104">**Märkus.** Kui teie seade või rakendus lakkas hiljaaegu töötamast, võtke arvesse, et alustasime hiljaaegu plaanipäraselt [3DES-šifri keelamist](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="63914-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="63914-105">Mõjutatud seadmete kuvamiseks avage [SMTP autentimise kliendi aruanne](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="63914-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="63914-106">Levinud tõrgete seas on autentimistõrked ja autentimise nurjumised, TLS-i tõrge või nurjumine, šifrialgoritmi tõrge, algoritmide lahknevus või ühenduse katkemine.</span><span class="sxs-lookup"><span data-stu-id="63914-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="63914-107">Probleemi lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="63914-107">To resolve the issue:</span></span>

 - <span data-ttu-id="63914-108">**Windows Server 2003 IIS SMTP enam ei tööta. Vaja on uuemat Windowsi versiooni.**</span><span class="sxs-lookup"><span data-stu-id="63914-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="63914-109">Uurige oma rakenduse või seadme tarnija käest, kas rakendus või seade toetab mõnda tänapäevast šifrit või kas selle jaoks on olemas värskendus.</span><span class="sxs-lookup"><span data-stu-id="63914-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
