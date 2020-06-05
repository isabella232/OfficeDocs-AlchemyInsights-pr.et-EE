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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581871"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="91402-102">Microsoft 365 rakenduste parandamine "me ei saa ühendust kohe" sõnum</span><span class="sxs-lookup"><span data-stu-id="91402-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="91402-103">Kui kuvatakse see teade, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="91402-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="91402-104">Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="91402-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="91402-105">Vaadake [Microsofti URL-e ja IP-aadresside vahemikku](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="91402-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="91402-106">**Start**  >  **Run**ja seejärel tippige **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="91402-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="91402-107">Veenduge, et järgmised teenused on kõik töötavad:</span><span class="sxs-lookup"><span data-stu-id="91402-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="91402-108">Võrgu ühendatud seadmed auto-setup</span><span class="sxs-lookup"><span data-stu-id="91402-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="91402-109">Võrguloendi teenus</span><span class="sxs-lookup"><span data-stu-id="91402-109">Network List Service</span></span>
    - <span data-ttu-id="91402-110">Võrgukoha teadlikkus</span><span class="sxs-lookup"><span data-stu-id="91402-110">Network Location Awareness</span></span>
    - <span data-ttu-id="91402-111">Windowsi sündmuselogi</span><span class="sxs-lookup"><span data-stu-id="91402-111">Windows Event Log</span></span>

<span data-ttu-id="91402-112">Kui üks neist teenustest ei tööta, proovige käivitada.</span><span class="sxs-lookup"><span data-stu-id="91402-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="91402-113">Kui teil on probleem teenuse käivitamine, käivitage järgmine käsk, avades käsuviiba laiendatud õigustega:</span><span class="sxs-lookup"><span data-stu-id="91402-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="91402-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="91402-114">**sfc /scannow**</span></span>

<span data-ttu-id="91402-115">Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="91402-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="91402-116">Üksikasjalikku teavet leiate jaotisest ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovige hiljem uuesti "tõrge, kui aktiveerite Office ' i Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="91402-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>