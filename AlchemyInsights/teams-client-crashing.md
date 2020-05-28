---
title: Kas Teamsi klient jookseb kokku?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354048"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="86205-102">Kas Teamsi klient jookseb kokku?</span><span class="sxs-lookup"><span data-stu-id="86205-102">Teams client crashing?</span></span>

<span data-ttu-id="86205-103">Kui teie Teamsi klient jookseb kokku, proovige järgmist.</span><span class="sxs-lookup"><span data-stu-id="86205-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="86205-104">Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="86205-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="86205-105">Veenduge, et kõik [Microsoft 365 URL-id ja aadressivahemikud](https://docs.microsoft.com/microsoftteams/connectivity-issues) on juurdepääsetavad.</span><span class="sxs-lookup"><span data-stu-id="86205-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="86205-106">Logige sisse oma rentniku administraatori kontoga ja kontrollige oma [teenuse tervise armatuurlauale](https://docs.microsoft.com/office365/enterprise/view-service-health) veendumaks, et katkestust või teenuse halvenemine on olemas.</span><span class="sxs-lookup"><span data-stu-id="86205-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="86205-107">Desinstallige ja installige meeskonnad rakendus (link)</span><span class="sxs-lookup"><span data-stu-id="86205-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="86205-108">Sirvige arvutis kausta%appdata%\Microsoft\teams\ ja kustutage kõik selle kausta failid.</span><span class="sxs-lookup"><span data-stu-id="86205-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="86205-109">[Laadige alla ja installige meeskonnad app](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ja võimaluse korral installige meeskonnad administraatorina (paremklõps meeskonnad Installer ja valige "Käivita administraatorina" Kui saadaval).</span><span class="sxs-lookup"><span data-stu-id="86205-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="86205-110">Kui teie meeskonnad klient ikka krahhi, saate probleemi taasesitada?</span><span class="sxs-lookup"><span data-stu-id="86205-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="86205-111">Kui jah, siis:</span><span class="sxs-lookup"><span data-stu-id="86205-111">If so:</span></span>

1. <span data-ttu-id="86205-112">Juhiste Salvesti abil saate oma sammud jäädvustada.</span><span class="sxs-lookup"><span data-stu-id="86205-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="86205-113">Sulgege kõik mittevajalikud või konfidentsiaalsed rakendused.</span><span class="sxs-lookup"><span data-stu-id="86205-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="86205-114">Käivitage toimingute salvesti ja paljundada probleem mõjutatud kasutajakonto sisse logitud.</span><span class="sxs-lookup"><span data-stu-id="86205-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="86205-115">[Koguda meeskonnad logid, mis jäädvustada salvestatud reprodutseerida sammud](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="86205-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="86205-116">**Märkus**: Veenduge, et jäädvustada mõjutatud kasutaja sisselogimise aadress.</span><span class="sxs-lookup"><span data-stu-id="86205-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="86205-117">Koguge mälutõmmise ja/või rikke kopp info (Windows).</span><span class="sxs-lookup"><span data-stu-id="86205-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="86205-118">Käivitage Windows PowerShelli arvutis, kus crash esineb ja käivitage järgmised käsud:</span><span class="sxs-lookup"><span data-stu-id="86205-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="86205-119">Kinnitage fail oma tugiteenuse teenindusjuhtumile.</span><span class="sxs-lookup"><span data-stu-id="86205-119">Attach the file to your support case.</span></span>
