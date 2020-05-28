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
# <a name="teams-client-crashing"></a>Kas Teamsi klient jookseb kokku?

Kui teie Teamsi klient jookseb kokku, proovige järgmist.

- Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Veenduge, et kõik [Microsoft 365 URL-id ja aadressivahemikud](https://docs.microsoft.com/microsoftteams/connectivity-issues) on juurdepääsetavad.

- Logige sisse oma rentniku administraatori kontoga ja kontrollige oma [teenuse tervise armatuurlauale](https://docs.microsoft.com/office365/enterprise/view-service-health) veendumaks, et katkestust või teenuse halvenemine on olemas.

- Desinstallige ja installige meeskonnad rakendus (link)
    - Sirvige arvutis kausta%appdata%\Microsoft\teams\ ja kustutage kõik selle kausta failid.
    - [Laadige alla ja installige meeskonnad app](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ja võimaluse korral installige meeskonnad administraatorina (paremklõps meeskonnad Installer ja valige "Käivita administraatorina" Kui saadaval).

Kui teie meeskonnad klient ikka krahhi, saate probleemi taasesitada? Kui jah, siis:

1. Juhiste Salvesti abil saate oma sammud jäädvustada.
    - Sulgege kõik mittevajalikud või konfidentsiaalsed rakendused.
    - Käivitage toimingute salvesti ja paljundada probleem mõjutatud kasutajakonto sisse logitud.
    - [Koguda meeskonnad logid, mis jäädvustada salvestatud reprodutseerida sammud](https://docs.microsoft.com/microsoftteams/log-files). **Märkus**: Veenduge, et jäädvustada mõjutatud kasutaja sisselogimise aadress.
    - Koguge mälutõmmise ja/või rikke kopp info (Windows). Käivitage Windows PowerShelli arvutis, kus crash esineb ja käivitage järgmised käsud:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Kinnitage fail oma tugiteenuse teenindusjuhtumile.
