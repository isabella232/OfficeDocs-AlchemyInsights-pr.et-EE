---
title: Juurutamine Microsoft 365 apps ettevõtte ühiskasutuses kasutamiseks RDS, Terminal Server või VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704701"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Juurutamine Microsoft 365 apps ettevõtte ühiskasutuses kasutamiseks RDS, Terminal Server või VDI

Juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste (RDS), varem nimega terminaliteenused:
- Peab teil olema Microsoft 365 äriplaan või Office 365 kava, mis sisaldab Microsoft 365 apps Enterprise, näiteks Office 365 Enterprise E3 või Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 apps äri ja Microsoft 365 Business Premium Standard plaanid ei sisalda Microsoft 365 apps Enterprise.
- Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Samuti saate alla laadida ja käivitada [Microsofti toe ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Microsoft 365 apps Enterprise ühiskasutatava arvuti aktiveerimise režiimis.

Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks toimige järgmiselt.
- Vaadake [tõrkeotsingu probleemid ühiskasutusse antud arvuti aktiveerimine Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Lugege artiklit [Microsoft 365 suurettevõtterakenduste aktiveerimisoleku lähtestamine](https://go.microsoft.com/fwlink/?linkid=2109218) (inglise keeles).

Kui soovite installida Microsoft 365 apps Enterprise RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, toimige järgmiselt:

1.    Kontrollige, mis tellimus teil on. [Õpi, kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Vajadusel aktiveerige mõni muu tellimus. [Õpi, kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Kui Office on juba installitud RDS-serverisse, kasutades muid Microsofti tellimusi, desinstallige see. Näiteks, **minnes** > juhtpaneeli**desinstallida programmi**. Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.
4.    RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige microsoft 365 apps Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.
6.    RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:
   1. Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige **Käivita**. Väljale Ava tippige **käsk regedit**ja seejärel valige **OK**.
   2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .
   3. Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et jagatud arvuti aktiveerimine on lubatud Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

