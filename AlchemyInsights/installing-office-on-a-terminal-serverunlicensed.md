---
title: Office ' i installimine terminaliserveri – litsentsimata
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663113"
---
# <a name="installing-office-on-a-terminal-server"></a>Office ' i installimine terminaliserveri

Rakenduse Microsoft 365 for Enterprise for Enterprise Windowsi serverile juurutamiseks kaugtöölaua teenuste (RDS), varem nimega terminaliteenuste kaudu.
  
- Teil peab olema Microsoft 365 tellimus, mis sisaldab Enterprise ' i jaoks mõeldud Microsoft 365 rakendusi (nt Office 365 Enterprise E3 või Enterprise E5). Microsoft 365 rakendused ettevõtetele ja Microsoft 365 for Premiumi lepingud ei sisalda Microsoft 365 Enterprise ' i jaoks mõeldud rakendusi.

- Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Kui soovite installida Microsoft 365 rakendusi RDS-ile Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätteid***, kasutage järgmisi juhiseid.

> [!TIP]
> Samuti saate alla laadida ja käivitada [Microsofti tugiteenuste ja taastekonsooli abilise](https://aka.ms/SaRA_OfficeSCA_M365Portal) , et installida Office ' i ühiskasutusega arvuti aktiveerimise režiimis Microsoft 365 rakendused.
  
1. Vaadake, milline Microsoft 365 tellimus teil on. [Uurige, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Vajadusel aktiveerige mõni muu Microsoft 365 tellimus. [Uurige, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Kui Office on juba RDS-serverisse installitud mis tahes muu Microsoft 365 tellimuse abil, desinstallige see. Näiteks juhtpaneeli käsuga \> Desinstalli programm. Kui teil on probleeme, desinstallige [Microsoft support ja Recovery Assistanti](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.

4. Rakenduses RDS logige sisse oma administraatori kontoga Microsoft 365 halduskeskus ja [installige Enterprise ' i jaoks microsoft 365](https://portal.office.com/OLS/MySoftware.aspx)' i rakendused.

5. Kui Office on installitud, ***Ärge avage ega logige sisse*** ühtegi Office ' i rakendusse.

6. RDS-serveris lubage ühiskasutusega arvuti aktiveerimine, redigeerides registrit, järgides järgmisi juhiseid.

1. Paremklõpsake ekraani vasakus allnurgas olevat nuppu Windows ja valige Käivita. Tippige väljale Ava **käsk regedit**ja seejärel klõpsake nuppu OK.

2. Kui teilt küsitakse, kas soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige Jah.

3. Lisage registriredaktori **SharedComputerLicensing** stringi väärtus, mille sätteks on HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. RDS-serveris ***logige sisse lõppkasutajana*** ja veenduge, [et ühiskasutusega arvuti aktiveerimine oleks lubatud Microsoft 365 rakenduste jaoks Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)' i jaoks.

Lisateavet Office ' i juurutamise tööriista funktsioonide, häälestamise juhiste ja kohandatud installide juhiste kohta leiate teemast Office ' i juurutamise tööriista kasutamine rakenduses [Microsoft 365 Apps for Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks lugege teemat [ühiskasutusega arvuti aktiveerimisega seotud probleemide tõrkeotsing Enterprise ' i jaoks mõeldud Microsoft 365 rakenduste jaoks](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  