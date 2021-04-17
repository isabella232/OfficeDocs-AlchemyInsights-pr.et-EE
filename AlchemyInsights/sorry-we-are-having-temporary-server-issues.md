---
title: Microsoft 365 rakenduste parandamine Kahjuks on meil ajutiste serveriprobleemide teade
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835267"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="a835b-102">Microsoft 365 rakenduste "Kahjuks on meil ajutised serveriprobleemid" parandamine</span><span class="sxs-lookup"><span data-stu-id="a835b-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="a835b-103">Kui teile kuvatakse see teade, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="a835b-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a835b-104">Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="a835b-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a835b-105">Vt [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a835b-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a835b-106">Avage Start Run  >  **(Käivita)** ja seejärel tippige **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="a835b-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a835b-107">Veenduge, et kõik järgmised teenused töötaks.</span><span class="sxs-lookup"><span data-stu-id="a835b-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a835b-108">Võrguühendusega seadmete automaathäälestus</span><span class="sxs-lookup"><span data-stu-id="a835b-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a835b-109">Võrguteenus</span><span class="sxs-lookup"><span data-stu-id="a835b-109">Network List Service</span></span>
    - <span data-ttu-id="a835b-110">Võrguasukoha teadlikkus</span><span class="sxs-lookup"><span data-stu-id="a835b-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a835b-111">Windowsi sündmuste logi</span><span class="sxs-lookup"><span data-stu-id="a835b-111">Windows Event Log</span></span>

<span data-ttu-id="a835b-112">Kui mõni neist teenustest ei tööta, proovige seda käivitada.</span><span class="sxs-lookup"><span data-stu-id="a835b-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a835b-113">Kui teil on teenuse käivitamisel probleeme, käivitage järgmine käsk, avades administraatoriõigustega käsuviiba.</span><span class="sxs-lookup"><span data-stu-id="a835b-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a835b-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="a835b-114">**sfc /scannow**</span></span>

<span data-ttu-id="a835b-115">Pärast selle käsu lõpule viimist taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="a835b-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a835b-116">Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Proovige hiljem uuesti" tõrge, kui aktiveerite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a835b-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>