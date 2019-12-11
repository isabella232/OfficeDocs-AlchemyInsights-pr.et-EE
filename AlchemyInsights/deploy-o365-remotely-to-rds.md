---
title: Juurutamine Office 365 ProPlus ühiskasutuses kasutamiseks RDS, Terminal Server või VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959456"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Juurutamine Office 365 ProPlus ühiskasutuses kasutamiseks RDS, Terminal Server või VDI

Office 365 ProPlusi juurutamine kaugtöölaua teenuste (RDS), varem nimega Terminal Services abil:
- Peab teil olema Microsoft 365 äriplaan või Office 365 kava, mis sisaldab Office 365 ProPlus, näiteks Office 365 Enterprise E3 või Enterprise E5.
   > [!NOTE] 
   > Office 365 Business ja Office 365 Business Premiumi plaanid ei sisalda Office 365 ProPlus.
- Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Samuti saate alla laadida ja käivitada [Microsoft support ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Office 365 ProPlus jagatud arvuti aktiveerimise režiimis.

Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutamine office 365 ProPlus kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks toimige järgmiselt.
- Vaadake [tõrkeotsingu probleemid ühiskasutusse antud arvuti aktiveerimine Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Vt [Lähtesta Office 365 ProPlus aktiveerimise olek](https://go.microsoft.com/fwlink/?linkid=2109218).

Kui soovite installida Office 365 ProPlus RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, toimige järgmiselt:

1.  Kontrollige, milline Office 365 plaan teil on. [Õpi, kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Vajadusel aktiveerige mõni muu Office 365 plaan. [Õpi, kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Kui Office on juba installitud RDS server, kasutades muid Office 365 plaanid, desinstallige see. Näiteks, **minnes** > juhtpaneeli**desinstallida programmi**. Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.
4.  RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.
6.  RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:
   1. Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige **Käivita**. Väljale Ava tippige **käsk regedit**ja seejärel valige **OK**.
   2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .
   3. Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et ühiskasutuses arvuti aktiveerimine on lubatud Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

