---
title: Microsoft 365 rakenduste parandamine Ei leidnud office'i litsentsidega seotud sõnumit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816484"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="69453-102">Microsoft 365 rakenduste parandamine sõnumiga "Ei leidnud seotud office'i litsentse"</span><span class="sxs-lookup"><span data-stu-id="69453-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="69453-103">Kui teile kuvatakse see teade, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="69453-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="69453-104">Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="69453-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="69453-105">Vt [Microsoft 365 URL-id ja IP-aadresside vahemikud.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="69453-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="69453-106">Eemaldage [mõjutatud kasutaja Office'i litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määrake see ümber.</span><span class="sxs-lookup"><span data-stu-id="69453-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="69453-107">Avage Office'i rakendus [ja logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mis tahes olemasolevast kasutajakontost.</span><span class="sxs-lookup"><span data-stu-id="69453-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="69453-108">Avage Windowsi sätted >   >  **Meilikontod & kontod** ja eemaldage kõik töökontod peale mõjutatud konto.</span><span class="sxs-lookup"><span data-stu-id="69453-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="69453-109">Avage Windowsi sätted >   >  **Kontod Accessi töö- või koolikonto** ja katkestage ühendus kõigi töökontodega, v.a mõjutatud konto.</span><span class="sxs-lookup"><span data-stu-id="69453-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="69453-110">Lähtestage Office'i aktiveerimisolekut.</span><span class="sxs-lookup"><span data-stu-id="69453-110">Reset the Office activation state.</span></span> <span data-ttu-id="69453-111">[Vaadake, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="69453-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="69453-112">[Logige sisse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakontoga.</span><span class="sxs-lookup"><span data-stu-id="69453-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="69453-113">Lisateavet tõrkeotsingulahenduste kohta leiate teemast [Litsentsimata toote- ja aktiveerimistõrked Office's.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="69453-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>