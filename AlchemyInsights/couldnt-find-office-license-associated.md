---
title: Microsoft 365 rakenduste parandamine ei leia Office ' i litsentsidega seostuvat sõnumit
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747691"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="1285b-102">Microsoft 365 rakenduste parandamine "ei saanud Office ' i litsentsidega seostuvat teadet"</span><span class="sxs-lookup"><span data-stu-id="1285b-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="1285b-103">Kui teile kuvatakse see teade, proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="1285b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="1285b-104">Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="1285b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="1285b-105">Vaadake teemat [Microsoft 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="1285b-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="1285b-106">Eemaldage mõjutatud kasutaja [Office ' i litsents ja määrake see](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) uuesti.</span><span class="sxs-lookup"><span data-stu-id="1285b-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="1285b-107">Avage Office ' i rakendus ja [logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost.</span><span class="sxs-lookup"><span data-stu-id="1285b-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="1285b-108">Avage Windowsi sätted > **kontode**  >  **Meilikontod & kontod**ja eemaldage kõik töökontod, v. a mõjutatud konto.</span><span class="sxs-lookup"><span data-stu-id="1285b-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="1285b-109">Avage Windowsi sätted > **kontode**  >  **juurdepääs tööle või koolile**ning kõigi Töökontode, v. a mõjutatud kontoga ühenduse katkestamine.</span><span class="sxs-lookup"><span data-stu-id="1285b-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="1285b-110">Lähtestage Office ' i aktiveerimise olek.</span><span class="sxs-lookup"><span data-stu-id="1285b-110">Reset the Office activation state.</span></span> <span data-ttu-id="1285b-111">[Vaadake, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="1285b-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="1285b-112">[Logige](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sisse mõjutatud kasutaja kontoga.</span><span class="sxs-lookup"><span data-stu-id="1285b-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="1285b-113">Täiendavate lahenduste leidmiseks lugege artiklit [Office ' i litsentsimata toodete ja aktiveerimise tõrgete](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)tõrkeotsing.</span><span class="sxs-lookup"><span data-stu-id="1285b-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>