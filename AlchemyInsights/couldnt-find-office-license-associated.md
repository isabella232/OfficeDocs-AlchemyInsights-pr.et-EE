---
title: Microsoft 365 rakenduste parandamine ei leidnud Office ' i litsentsid seotud sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580437"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="b4391-102">Microsoft 365 rakenduste kinnitamine "ei leidnud Office ' i litsentsid seotud" sõnum</span><span class="sxs-lookup"><span data-stu-id="b4391-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="b4391-103">Kui kuvatakse see teade, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="b4391-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b4391-104">Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="b4391-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b4391-105">Vt [microsofti 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="b4391-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="b4391-106">Eemaldage ja [määrata mõjutatud kasutaja Office ' i litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) .</span><span class="sxs-lookup"><span data-stu-id="b4391-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="b4391-107">Avage Office ' i rakendus ja [logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) kõigist olemasolevatest kasutajakontodest.</span><span class="sxs-lookup"><span data-stu-id="b4391-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="b4391-108">Avage Windowsi sätted > **kontod**  >  **e-posti & kontod**ja eemaldage kõik töökontod, välja arvatud mõjutatud konto.</span><span class="sxs-lookup"><span data-stu-id="b4391-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="b4391-109">Avage Windowsi sätted > **kontod**  >  **juurdepääsu töö või kooli**ja katkestada kõik töö kontod, välja arvatud mõjutatud konto.</span><span class="sxs-lookup"><span data-stu-id="b4391-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="b4391-110">Lähtestage Office ' i aktiveerimisolek.</span><span class="sxs-lookup"><span data-stu-id="b4391-110">Reset the Office activation state.</span></span> <span data-ttu-id="b4391-111">[Õpi, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="b4391-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="b4391-112">[Logige sisse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakonto abil.</span><span class="sxs-lookup"><span data-stu-id="b4391-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="b4391-113">Täiendavate tõrkeotsingulahenduste saamiseks vaadake [Office ' i litsentseerimata toote-ja aktiveerimistõrkeid](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="b4391-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>