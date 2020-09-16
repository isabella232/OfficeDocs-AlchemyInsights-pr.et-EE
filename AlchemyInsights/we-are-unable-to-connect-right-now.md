---
title: Aktiveerimise probleem – me ei saa kohe ühendust luua
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725979"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="7cf95-102">Microsoft 365 rakenduste parandamine "me ei saa praegu ühendust luua".</span><span class="sxs-lookup"><span data-stu-id="7cf95-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="7cf95-103">Kui teile kuvatakse see teade, proovige teha järgmist.</span><span class="sxs-lookup"><span data-stu-id="7cf95-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="7cf95-104">Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele.</span><span class="sxs-lookup"><span data-stu-id="7cf95-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="7cf95-105">Lugege teemat [Microsofti URL-ide ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="7cf95-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="7cf95-106">Avage **Start**  >  **Run**ja tippige tekst **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="7cf95-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="7cf95-107">Veenduge, et kõik töötavad järgmised teenused.</span><span class="sxs-lookup"><span data-stu-id="7cf95-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="7cf95-108">Võrguga ühendatud seadmete automaatne häälestamine</span><span class="sxs-lookup"><span data-stu-id="7cf95-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="7cf95-109">Võrgu loendi teenus</span><span class="sxs-lookup"><span data-stu-id="7cf95-109">Network List Service</span></span>
    - <span data-ttu-id="7cf95-110">Võrgu asukoha teadlikkus</span><span class="sxs-lookup"><span data-stu-id="7cf95-110">Network Location Awareness</span></span>
    - <span data-ttu-id="7cf95-111">Windowsi sündmuste logi</span><span class="sxs-lookup"><span data-stu-id="7cf95-111">Windows Event Log</span></span>

<span data-ttu-id="7cf95-112">Kui mõni neist teenustest ei tööta, proovige seda käivitada.</span><span class="sxs-lookup"><span data-stu-id="7cf95-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="7cf95-113">Kui teil on teenuse käivitamise probleem, käivitage järgmine käsk, avades käsuviiba, kus on kõrgendatud õigused.</span><span class="sxs-lookup"><span data-stu-id="7cf95-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="7cf95-114">**SFC/scannow**</span><span class="sxs-lookup"><span data-stu-id="7cf95-114">**sfc /scannow**</span></span>

<span data-ttu-id="7cf95-115">Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.</span><span class="sxs-lookup"><span data-stu-id="7cf95-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="7cf95-116">Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Kui aktiveerite Office ' i Microsoft 365 kaudu, proovige hiljem uuesti](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="7cf95-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>