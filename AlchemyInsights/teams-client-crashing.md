---
title: Kas Teamsi klient jookseb kokku?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826267"
---
# <a name="teams-client-crashing"></a>Kas Teamsi klient jookseb kokku?

Kui teie Teamsi klient jookseb kokku, proovige järgmist.

- Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Veenduge, et kõik [Microsoft 365 URL-id ja aadressivahemikud on](https://docs.microsoft.com/microsoftteams/connectivity-issues) juurdepääsetavad.

- Logige sisse oma rentnikuadministraatori kontoga ja kontrollige teenuse [seisundi armatuurlauda,](https://docs.microsoft.com/office365/enterprise/view-service-health) et veenduda, et teenusekatkestust ega teenuse halvenemist ei esine.

- Teamsi rakenduse desinstallimine ja uuesti installimine (link)
    - Liikuge sirvides oma arvuti kaustani %appdata%\Microsoft\teams\ ja kustutage kõik selles kataloogis olevad failid.
    - [Laadige alla ja installige Teamsi rakendus](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ning võimalusel installige Teams administraatorina (paremklõpsake Teamsi installerit ja valige "Käivita administraatorina", kui see on saadaval).

Kui teie Teamsi klientrakendus ikka jookseb kokku, kas saate probleemi uuesti esile tada? Kui jah, siis:

1. Juhiste salvesti abil saate oma toimingud jäädvustada.
    - Sulgege kõik mittevajalikud või konfidentsiaalsed rakendused.
    - Käivitage toimingute salvesti ja paljundada probleem mõjutatud kasutajakontoga sisse logides.
    - [Koguge töörühmade logid, mis jäädvustavad salvestatud repro etapid.](https://docs.microsoft.com/microsoftteams/log-files) **Märkus.** Veenduge, et jäädvustate mõjutatud kasutaja sisselogimisaadressi.
    - Koguge tõmmise- ja/või tõrkeämbri teave (Windows). Käivitage Windows Powershell seadmes, kus krahh toimub, ja käivitage järgmised käsud.

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Manustage fail tugiteenuste juhtumile.
