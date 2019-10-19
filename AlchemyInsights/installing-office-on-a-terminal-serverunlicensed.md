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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205405"
---
# <a name="installing-office-on-a-terminal-server"></a>Office ' i installimine terminaliserverisse

Office 365 ProPlusi juurutamine Windows Serveri abil kaugtöölaua teenuste (RDS), varem nimega Terminal Services:
  
- Peab teil olema Office 365 kava, mis sisaldab Office 365 ProPlus, näiteks Office 365 Enterprise E3 või Enterprise E5. Office 365 Business ja Office 365 Business Premiumi plaanid ei sisalda Office 365 ProPlus.

- Peate lubama [ühiskasutusega arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Kui soovite installida Office 365 ProPlus RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, kasutage järgmisi samme.

> [!TIP]
> Samuti saate alla laadida ja käivitada [Microsoft support ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Office 365 ProPlus jagatud arvuti aktiveerimise režiimis.
  
1. Kontrollige, milline Office 365 plaan teil on. [Vaadake, kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Vajadusel aktiveerige mõni muu Office 365 plaan. [Vaadake, kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Kui Office on juba installitud RDS server, kasutades muid Office 365 plaanid, desinstallige see. Näiteks, minnes juhtpaneeli \> desinstallida programmi. Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.

4. RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.

6. RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:

1. Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige käsk Käivita. Väljale Ava tippige **käsk regedit**ja seejärel valige OK.

2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige Jah.

3. Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 all HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et ühiskasutuses arvuti aktiveerimine on lubatud Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutamine office 365 ProPlus kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks vaadake teemat probleemide [tõrkeotsing ühiskasutusse antud arvuti aktiveerimisega Office 365 ProPlusi jaoks](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  