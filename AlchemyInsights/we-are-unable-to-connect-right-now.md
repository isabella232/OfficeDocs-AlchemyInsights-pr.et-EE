---
title: Aktiveerimisprobleem – me ei saa praegu ühendust luua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716168"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="c9860-102">Office ' i rakenduste parandamine "me ei saa ühendust kohe" sõnum</span><span class="sxs-lookup"><span data-stu-id="c9860-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="c9860-103">Kui kuvatakse see teade, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="c9860-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="c9860-104">Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Office ' i rakendustele Interneti-ühendust.</span><span class="sxs-lookup"><span data-stu-id="c9860-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="c9860-105">Vaadake [Microsofti URL-e ja IP-aadresside vahemikku](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="c9860-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="c9860-106">**Start** > **Run**ja seejärel tippige **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="c9860-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="c9860-107">Veenduge, et järgmised teenused on kõik töötavad:</span><span class="sxs-lookup"><span data-stu-id="c9860-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="c9860-108">Võrgu ühendatud seadmed auto-setup</span><span class="sxs-lookup"><span data-stu-id="c9860-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="c9860-109">Võrguloendi teenus</span><span class="sxs-lookup"><span data-stu-id="c9860-109">Network List Service</span></span>
    - <span data-ttu-id="c9860-110">Võrgukoha teadlikkus</span><span class="sxs-lookup"><span data-stu-id="c9860-110">Network Location Awareness</span></span>
    - <span data-ttu-id="c9860-111">Windowsi sündmuselogi</span><span class="sxs-lookup"><span data-stu-id="c9860-111">Windows Event Log</span></span>

<span data-ttu-id="c9860-112">Kui üks neist teenustest ei tööta, proovige käivitada.</span><span class="sxs-lookup"><span data-stu-id="c9860-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="c9860-113">Kui teil on probleem teenuse käivitamine, käivitage järgmine käsk, avades käsuviiba laiendatud õigustega:</span><span class="sxs-lookup"><span data-stu-id="c9860-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="c9860-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="c9860-114">**sfc /scannow**</span></span>

<span data-ttu-id="c9860-115">Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="c9860-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="c9860-116">Üksikasjalikku teavet leiate jaotisest ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovige hiljem uuesti "tõrge, kui aktiveerite Office ' i Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="c9860-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>