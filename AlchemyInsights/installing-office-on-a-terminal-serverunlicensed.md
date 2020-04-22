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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763213"
---
# <a name="installing-office-on-a-terminal-server"></a>Office ' i installimine terminaliserverisse

Juurutamiseks Microsoft 365 apps Enterprise Windows Server kaugtöölaua teenuste (RDS), varem nimega Terminal Services kasutamisel:
  
- Teil peab olema Microsoft 365 tellimus, mis sisaldab Microsoft 365 apps Enterprise, nt Office 365 Enterprise E3 või Enterprise E5. Microsoft 365 apps äri ja Microsoft 365 apps Business Premium plaanid ei sisalda Microsoft 365 apps Enterprise.

- Peate lubama [ühiskasutusega arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Kui soovite installida Microsoft 365 apps Enterprise RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, kasutage järgmisi samme.

> [!TIP]
> Samuti saate alla laadida ja käivitada [Microsofti toe ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Microsoft 365 apps Enterprise ühiskasutatava arvuti aktiveerimise režiimis.
  
1. Kontrollige, mida Microsoft 365 tellimus teil on. [Vaadake, kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Vajadusel aktiveerige mõni muu Microsoft 365 tellimus. [Vaadake, kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Kui Office on juba installitud RDS server, kasutades muid Microsoft 365 tellimused, desinstallige see. Näiteks, minnes juhtpaneeli \> desinstallida programmi. Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.

4. RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige microsoft 365 apps Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.

6. RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:

1. Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige käsk Käivita. Väljale Ava tippige **käsk regedit**ja seejärel valige OK.

2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige Jah.

3. Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et jagatud arvuti aktiveerimine on lubatud Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks lugege [juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Ühiskasutatava arvuti aktiveerimisega seotud tõrgete lahendamiseks vaadake teemat [microsofti 365 rakenduste jaoks ühiskasutatava arvuti aktiveerimise tõrkeotsing](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  