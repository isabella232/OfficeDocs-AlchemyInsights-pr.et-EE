---
title: Teams lisandmoodul Mac-arvuti jaoks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582066"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="12c2a-102">Teams lisandmoodul Mac-arvuti jaoks</span><span class="sxs-lookup"><span data-stu-id="12c2a-102">Teams add-in for Mac</span></span>

<span data-ttu-id="12c2a-103">Maci opsüsteemi Teams puuduva lisandmooduli tõrkeotsinguks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="12c2a-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="12c2a-104">**1. juhis:** Kui teil on Exchange kohapealne hübriidautentimine (nõutav on 2016 CU3 või uuem), saate Test-HMA.ps1 tööriista abil kinnitada, et hübriid-modernautentimine on õigesti konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="12c2a-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="12c2a-105">Lisateavet leiate teemast Hübriidjuurutuse [modernautentimise häälestuse valideerimine Outlook iOS-i ja Androidi jaoks.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="12c2a-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="12c2a-106">**Märkus** Kasutage UPN-aadressivormingut (nt [username@contoso.com](mailto:username@contoso.com)), mitte domeeni\kasutajanime.</span><span class="sxs-lookup"><span data-stu-id="12c2a-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="12c2a-107">Tehke seda ka kasutajate jaoks, kellel Exchange Online postkastid.</span><span class="sxs-lookup"><span data-stu-id="12c2a-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="12c2a-108">**2. juhis.** Avage kasutaja **tööriistade**  >  **kontod**... ja Outlook mac-arvutis ning otsige üles ja valige konto.</span><span class="sxs-lookup"><span data-stu-id="12c2a-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="12c2a-109">Kinnitage, et loetletud kasutajanimi on UPN-vormingus [(nt username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="12c2a-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="12c2a-110">**3. juhis:** Veenduge, et kasutaja on litsentsitud Microsoft Teams kasutaja.</span><span class="sxs-lookup"><span data-stu-id="12c2a-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="12c2a-111">Kasutaja peab kasutama Office 365 for Maci tellimust, tooteversiooni 16.24 või uuemat versiooni.</span><span class="sxs-lookup"><span data-stu-id="12c2a-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>