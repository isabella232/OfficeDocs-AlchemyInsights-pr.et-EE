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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187717"
---
# <a name="teams-client-crashing"></a>Teams klientrakenduse krahh

Kui teie Teamsi klient jookseb kokku, proovige järgmist.

- Kui kasutate Teamsi töölauarakendust, [veenduge, et rakendus oleks täielikult värskendatud](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Veenduge, et [kõik Microsoft 365 URL-id ja aadressivahemikud on](/microsoftteams/connectivity-issues) juurdepääsetavad.

- Logige sisse oma rentnikuadministraatori kontoga ja kontrollige teenuse [seisundi armatuurlauda,](/office365/enterprise/view-service-health) et veenduda, et teenusekatkestust ega teenuse halvenemist ei esine.

- Desinstallige ja installige Teams uuesti
    - Liikuge sirvides oma arvuti kaustani %appdata%\Microsoft\Teams\ ja kustutage kõik selles kataloogis olevad failid.
    - [Laadige alla ja installige Teams rakendus](https://www.microsoft.com/microsoft-teams/download-app)ning võimalusel installige Teams administraatorina (paremklõpsake Teams installerit ja valige **Käivita** administraatorina, kui see on saadaval).

Kui teie Teams klientrakendus ikka jookseb kokku, proovige probleem uuesti esile leida. Kui saate teha:

1. Juhiste salvesti abil saate oma toimingud jäädvustada.
    - Sulgege kõik mittevajalikud või konfidentsiaalsed rakendused.
    - Käivitage toimingute salvesti ja paljundada probleem mõjutatud kasutajakontoga sisse logides.
    - [Koguge töörühmade logid, mis jäädvustavad salvestatud repro etapid.](/microsoftteams/log-files) **Märkus.** Veenduge, et jäädvustate mõjutatud kasutaja sisselogimisaadressi.
    - Koguge tõmmise- ja/või tõrkeämbri teave (Windows). Käivitage Windows powershell seadmes, kus krahh toimub, ja käivitage järgmised käsud (pärast iga käsku vajutage sisestusklahvi (Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Pärast tekstifaili loomist ja kuval kuvamist salvestage fail ja manustage see teenusetaotlusele. 
