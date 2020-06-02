---
title: Office ' i installimine terminaliserverisse-litsentsimata
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508624"
---
# <a name="installing-office-on-a-terminal-server"></a>Office ' i installimine terminaliserverisse

Juurutamiseks Microsoft 365 apps Enterprise Windows Server kaugtöölaua teenuste (RDS), varem nimega Terminal Services kasutamisel:
  
- Teil peab olema Microsoft 365 tellimus, mis sisaldab Microsoft 365 apps Enterprise, nt Office 365 Enterprise E3 või Enterprise E5. Microsoft 365 apps äri ja Microsoft 365 apps Business Premium plaanid ei sisalda Microsoft 365 apps Enterprise.

- Peate lubama [ühiskasutusega arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Kui soovite installida Microsoft 365 apps Enterprise RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, kasutage järgmisi samme.

> [!TIP]
> Samuti saate alla laadida ja käivitada [Microsofti toe ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Microsoft 365 apps Enterprise ühiskasutatava arvuti aktiveerimise režiimis.
  
1. Kontrollige, mida Microsoft 365 tellimus teil on. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Vajadusel aktiveerige mõni muu Microsoft 365 tellimus. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Kui Office on juba installitud RDS server, kasutades muid Microsoft 365 tellimused, desinstallige see. Näiteks, minnes juhtpaneeli \> desinstallida programmi. Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.

4. RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige microsoft 365 apps Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.

6. RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:

1. Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige käsk Käivita. Väljale Ava tippige **käsk regedit**ja seejärel valige OK.

2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige Jah.

3. Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et jagatud arvuti aktiveerimine on lubatud Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks lugege [juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Ühiskasutatava arvuti aktiveerimisega seotud tõrgete lahendamiseks vaadake teemat [microsofti 365 rakenduste jaoks ühiskasutatava arvuti aktiveerimise tõrkeotsing](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  