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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507582"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Juurutamine Microsoft 365 apps ettevõtte ühiskasutuses kasutamiseks RDS, Terminal Server või VDI

Juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste (RDS), varem nimega terminaliteenused:
- Peab teil olema Microsoft 365 äriplaan või Office 365 kava, mis sisaldab Microsoft 365 apps Enterprise, näiteks Office 365 Enterprise E3 või Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 apps äri ja Microsoft 365 Business Premium Standard plaanid ei sisalda Microsoft 365 apps Enterprise.
- Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Samuti saate alla laadida ja käivitada [Microsofti toe ja taastamise abimees](https://aka.ms/SaRA_OfficeSCA_M365Portal) installida Microsoft 365 apps Enterprise ühiskasutatava arvuti aktiveerimise režiimis.

Eeltingimused, setup juhiseid ja juhiseid kohandatud installi Office ' i juurutamise tööriista abil kohta lisateabe saamiseks vaadake [juurutada Microsoft 365 apps Enterprise kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks toimige järgmiselt.
- Vaadake [tõrkeotsingu probleemid ühiskasutusse antud arvuti aktiveerimine Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lugege artiklit [Microsoft 365 suurettevõtterakenduste aktiveerimisoleku lähtestamine](https://go.microsoft.com/fwlink/?linkid=2109218) (inglise keeles).

Kui soovite installida Microsoft 365 apps Enterprise RDS Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätted***, toimige järgmiselt:

1.    Kontrollige, mis tellimus teil on. [Õpi, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Vajadusel aktiveerige mõni muu tellimus. [Õpi, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Kui Office on juba installitud RDS-serverisse, kasutades muid Microsofti tellimusi, desinstallige see. Näiteks, **minnes juhtpaneeli**  >  **desinstallida programmi**. Kui teil on probleeme, desinstallige [Microsofti toe-ja Taasteabimehe](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.
4.    RDS server, logige sisse Microsoft 365 halduskeskus administraatori kontoga ja [installige microsoft 365 apps Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    Pärast Office ' i installimist ***Ärge avage ega logige sisse*** ühelegi Office ' i rakendustele.
6.    RDS server, lubage ühiskasutusse antud arvuti aktiveerimine registri redigeerimisel toimige järgmiselt:
   1. Paremklõpsake ekraani alumises vasakus nurgas asuvat Windowsi nuppu ja valige **Käivita**. Väljale Ava tippige **käsk regedit**ja seejärel valige **OK**.
   2. Kui küsitakse, kas Registriredaktor lubab teie seadmes muudatusi teha, valige **Jah** .
   3. Registriredaktoris lisada stringi väärtus **Sharedcomputerlicensing** sätte 1 alla HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS server, logige sisse ***lõppkasutaja*** ja [veenduge, et jagatud arvuti aktiveerimine on lubatud Microsoft 365 apps Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

