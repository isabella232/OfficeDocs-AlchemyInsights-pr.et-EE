---
title: Teams klientrakenduse krahh
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890334"
---
# <a name="teams-client-crashing"></a>Teams klientrakenduse krahh

Kui teie Teamsi klient jookseb kokku, proovige järgmist.

- Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Veenduge, et [Microsoft 365 URL-id ja aadressivahemikud](https://docs.microsoft.com/microsoftteams/connectivity-issues) oleks juurdepääsetavad.

- Logige sisse oma rentnikuadministraatori kontoga ja kontrollige teenuse [seisundi armatuurlauda,](https://docs.microsoft.com/office365/enterprise/view-service-health) et veenduda, et teenusekatkestust ega teenuse halvenemist ei esine.

- Desinstallige ja installige Teams uuesti
    - Liikuge sirvides oma arvuti kaustani %appdata%\Microsoft\Teams\ ja kustutage kõik selles kataloogis olevad failid.
    - [Laadige alla ja installige Teams rakendus](https://www.microsoft.com/microsoft-teams/download-app)ning võimalusel installige Teams administraatorina (paremklõpsake Teams installerit ja valige **Käivita** administraatorina,kui see on saadaval).

Kui teie Teams klientrakendus ikka jookseb kokku, proovige probleem uuesti esile leida. Kui saate teha:

1. Toimingute jäädvustamiseks kasutage juhiste salvestit.
    - Sulgege kõik mittevajalikud või konfidentsiaalsed rakendused.
    - Käivitage toimingute salvesti ja paljunege probleem mõjutatud kasutajakontoga sisse logides.
    - [Koguge töörühmade logid, mis jäädvustavad salvestatud repro etapid.](https://docs.microsoft.com/microsoftteams/log-files) **Märkus.** Veenduge, et jäädvustate mõjutatud kasutaja sisselogimisaadressi.
    - Koguge tõmmise- ja/või tõrkeämbri teave (Windows). Käivitage Windows powershell seadmes, kus krahh toimub, ja käivitage järgmised käsud (pärast iga käsku vajutage sisestusklahvi (Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kui tekstifail on loodud ja ekraanil kuvatakse, salvestage fail ja manustage see teenusetaotlusele. 
