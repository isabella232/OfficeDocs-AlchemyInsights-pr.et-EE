---
title: Teamsi lisandmoodul Maci jaoks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629519"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="905ce-102">Teamsi lisandmoodul Maci jaoks</span><span class="sxs-lookup"><span data-stu-id="905ce-102">Teams add-in for Mac</span></span>

<span data-ttu-id="905ce-103">Puuduvate Teamsi lisandmoodulite tõrkeotsinguks Mac-operatsioonisüsteemi kasutajate jaoks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="905ce-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="905ce-104">**1. juhis:** Kui teil on kohapeal hübriid Exchange ' i (2016 CU3 või uuem versioon), kasutage tööriista Test-HMA.ps1, et kinnitada, et hübriid-modernne autentimine on õigesti konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="905ce-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="905ce-105">Lisateavet leiate teemast [Outlook for iOS-i ja Androidi hübriidi kaasaegse autentimise häälestamise kinnitamine](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="905ce-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="905ce-106">**Märkus** Kasutage UPN-aadressi vormingut (nt [username@contoso.com](mailto:username@contoso.com)), mitte domain\username.</span><span class="sxs-lookup"><span data-stu-id="905ce-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="905ce-107">Tehke seda isegi kasutajate jaoks, kellel on Exchange Online ' i postkastid.</span><span class="sxs-lookup"><span data-stu-id="905ce-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="905ce-108">**Juhis 2:** Kas kasutaja on valmis kasutama **tööriistu**  >  **Accounts**... rakenduses Outlook for Mac ning konto leidmiseks ja valimiseks.</span><span class="sxs-lookup"><span data-stu-id="905ce-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="905ce-109">Kontrollige, kas loetletud kasutajanimi on UPN-vormingus (nt [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="905ce-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="905ce-110">**3. juhis:** Kinnita kasutaja on litsentseeritud Microsoft Teamsi kasutaja.</span><span class="sxs-lookup"><span data-stu-id="905ce-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="905ce-111">Kasutaja peab kasutama Office 365 for Mac tellimust, toote versiooni 16,24 või uuemat versiooni.</span><span class="sxs-lookup"><span data-stu-id="905ce-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>