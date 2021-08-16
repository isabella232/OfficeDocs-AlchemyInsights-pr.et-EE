---
title: RDS Microsoft 365 suurettevõtterakendused terminaliserveris või VDI-s ühiskasutuses kasutamiseks
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031474"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS Microsoft 365 suurettevõtterakendused terminaliserveris või VDI-s ühiskasutuses kasutamiseks

Kaugtöölaua Microsoft 365 suurettevõtterakendused (RDS) varem nimetatud terminaliteenuste juurutamiseks:

- Teil peab olema Microsoft 365 for Businessi leping või Office 365, mis sisaldab Microsoft 365 suurettevõtterakendused (nt Office 365 Enterprise E3 või Enterprise E5).
   > [!NOTE]
   > Need Microsoft 365 ettevõtterakendused ja Microsoft 365 Business Standard ei sisalda Microsoft 365 suurettevõtterakendused.
- Peate lubama [arvuti ühisaktiveerimise.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Samuti saate Microsoft tugi- ja taasteteenuste abiline [](https://aka.ms/SaRA_OfficeSCA_M365Portal) arvuti ühisaktiveerimisrežiimi Microsoft 365 suurettevõtterakendused käivitada.

Lisateavet eeltingimuste, häälestusjuhiste ja juhiste kohta kohandatud installide kohta leiate Office juurutamistööriista abil teemast [Microsoft 365 suurettevõtterakendused juurutamine kaugtöölaua teenuste abil.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Ühisarvuti aktiveerimisega seotud tõrgete lahendamiseks:

- Lugege [teemat Arvuti ühisaktiveerimisega seotud probleemide tõrkeotsing Microsoft 365 suurettevõtterakendused](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lugege artiklit [Microsoft 365 suurettevõtterakenduste aktiveerimisoleku lähtestamine](https://go.microsoft.com/fwlink/?linkid=2109218) (inglise keeles).

Kui soovite installida Microsoft 365 suurettevõtterakendused RDS-i Microsoft 365 halduskeskus, mis kasutab ***vaikeinstallisätteid,*** tehke järgmist.

1. Kontrollige, milline tellimus teil on. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Vajaduse korral aktiveerige muu tellimus. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Kui Office on RDS-i serverisse installitud mõne muu Microsofti tellimuse abil, desinstallige see. Näiteks valige Juhtpaneel Programmi  >  **desinstallimine.** Desinstallige [Microsoft tugi- ja taasteteenuste abiline,](https://aka.ms/SARA-OfficeUninstall-Alchemy) kui teil on probleeme.
4. Logige RDS-serveris oma administraatorikontoga sisse Microsoft 365 halduskeskus ja [installige Microsoft 365 suurettevõtterakendused](https://portal.office.com/OLS/MySoftware.aspx).
5. Pärast Office installimist ärge ***avage*** ega logige sisse ühtegi Office rakendusse.
6. Lubage RDS-serveris ühisarvuti aktiveerimine, redigeerides registrit, järgides järgmisi juhiseid.
   1. Paremklõpsake ekraani vasakus allnurgas Windows ja valige Käivita **.** Tippige väljale Ava käsk **regedit** ja seejärel valige **OK**.
   2. Kui **teil** palutakse lubada registriredaktoril oma seadmes muudatusi teha, valige Jah.
   3. Lisage registriredaktoris stringi väärtus **SharedComputerLicensing** sättega 1 jaotises HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. Logige RDS-serveris ***lõppkasutajana*** sisse ja veenduge, et ühisarvuti [aktiveerimine on](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)lubatud Microsoft 365 suurettevõtterakendused .
