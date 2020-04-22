---
title: Office ' i rakenduste parandamine Vabandust, meil on ajutised server Probleemid sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764113"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="f2d3a-102">Office ' i rakenduste parandamine "Vabandust, meil on ajutised serveriprobleemid" sõnum</span><span class="sxs-lookup"><span data-stu-id="f2d3a-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="f2d3a-103">Kui kuvatakse see teade, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="f2d3a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f2d3a-104">Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Office ' i rakendustele Interneti-ühendust.</span><span class="sxs-lookup"><span data-stu-id="f2d3a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="f2d3a-105">Vaadake [URL-e ja IP-aadresside vahemikku](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f2d3a-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f2d3a-106">**Start** > **Run**ja seejärel tippige **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="f2d3a-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f2d3a-107">Veenduge, et järgmised teenused on kõik töötavad:</span><span class="sxs-lookup"><span data-stu-id="f2d3a-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f2d3a-108">Võrgu ühendatud seadmed auto-setup</span><span class="sxs-lookup"><span data-stu-id="f2d3a-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f2d3a-109">Võrguloendi teenus</span><span class="sxs-lookup"><span data-stu-id="f2d3a-109">Network List Service</span></span>
    - <span data-ttu-id="f2d3a-110">Võrgukoha teadlikkus</span><span class="sxs-lookup"><span data-stu-id="f2d3a-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f2d3a-111">Windowsi sündmuselogi</span><span class="sxs-lookup"><span data-stu-id="f2d3a-111">Windows Event Log</span></span>

<span data-ttu-id="f2d3a-112">Kui üks neist teenustest ei tööta, proovige käivitada.</span><span class="sxs-lookup"><span data-stu-id="f2d3a-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f2d3a-113">Kui teil on probleem teenuse käivitamine, käivitage järgmine käsk, avades käsuviiba laiendatud õigustega:</span><span class="sxs-lookup"><span data-stu-id="f2d3a-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f2d3a-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="f2d3a-114">**sfc /scannow**</span></span>

<span data-ttu-id="f2d3a-115">Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="f2d3a-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f2d3a-116">Üksikasjalikku teavet leiate jaotisest ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovige hiljem uuesti "tõrge, kui aktiveerite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="f2d3a-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>