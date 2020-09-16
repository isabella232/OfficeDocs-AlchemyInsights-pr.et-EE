---
title: Microsoft 365 rakenduste parandamine Vabandust, meil on ajutine serveri probleemid sõnum
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758241"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="2a9b4-102">Microsoft 365 rakenduste parandamine "Kahjuks on meil ajutised serveri probleemid" sõnum</span><span class="sxs-lookup"><span data-stu-id="2a9b4-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="2a9b4-103">Kui teile kuvatakse see teade, proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="2a9b4-104">Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="2a9b4-105">Vaadake teemat [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="2a9b4-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="2a9b4-106">Avage **Start**  >  **Run**ja tippige tekst **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="2a9b4-107">Veenduge, et kõik töötavad järgmised teenused.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="2a9b4-108">Võrguga ühendatud seadmete automaatne häälestamine</span><span class="sxs-lookup"><span data-stu-id="2a9b4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="2a9b4-109">Võrgu loendi teenus</span><span class="sxs-lookup"><span data-stu-id="2a9b4-109">Network List Service</span></span>
    - <span data-ttu-id="2a9b4-110">Võrgu asukoha teadlikkus</span><span class="sxs-lookup"><span data-stu-id="2a9b4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="2a9b4-111">Windowsi sündmuste logi</span><span class="sxs-lookup"><span data-stu-id="2a9b4-111">Windows Event Log</span></span>

<span data-ttu-id="2a9b4-112">Kui mõni neist teenustest ei tööta, proovige seda käivitada.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="2a9b4-113">Kui teil on teenuse käivitamise probleem, käivitage järgmine käsk, avades käsuviiba, kus on kõrgendatud õigused.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="2a9b4-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="2a9b4-114">**sfc /scannow**</span></span>

<span data-ttu-id="2a9b4-115">Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="2a9b4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="2a9b4-116">Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovi hiljem uuesti, kui aktiveerid](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="2a9b4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>