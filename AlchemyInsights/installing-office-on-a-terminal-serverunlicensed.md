---
title: Office'i installimine terminaliserverisse – litsentsimata
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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321995"
---
# <a name="installing-office-on-a-terminal-server"></a>Office installimine terminaliserverisse

Serveri Microsoft 365 suurettevõtterakendused juurutamiseks Windows kaugtöölaua teenuste (RDS) abil, mida varem nimetati terminaliteenusteks.
  
- Teil peab olema Microsoft 365 tellimus, mis sisaldab Microsoft 365 suurettevõtterakendused (nt Office 365 Enterprise E3 või Enterprise E5). Need Microsoft 365 ettevõtterakendused ja Microsoft 365 ettevõtterakendused Premium ei sisalda Microsoft 365 suurettevõtterakendused.

- Peate lubama arvuti [ühisaktiveerimise.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Kui soovite installida Microsoft 365 suurettevõtterakendused RDS-i Microsoft 365 halduskeskus, mis kasutab ***vaikeinstallisätteid,*** tehke järgmist.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Kontrollige, Microsoft 365 tellimus teil on. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Vajaduse korral aktiveerige muu Microsoft 365 tellimus. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Kui Office on RDS-i serverisse installitud mõne muu Microsoft 365 kaudu, desinstallige see. Näiteks valige Juhtpaneel Programmi \> desinstallimine. Desinstallige [Microsoft tugi- ja taasteteenuste abiline,](https://aka.ms/SARA-OfficeUninstall-Alchemy) kui teil on probleeme.

4. Logige RDS-serveris oma administraatorikontoga sisse Microsoft 365 halduskeskus ja [installige Microsoft 365 suurettevõtterakendused](https://portal.office.com/OLS/MySoftware.aspx).

5. Pärast Office installimist ***ärge avage*** ega logige sisse ühtegi Office rakendusse.

6. Lubage RDS-serveris ühisarvuti aktiveerimine, redigeerides registrit, järgides järgmisi juhiseid.

1. Paremklõpsake ekraani Windows vasakus allnurgas olevat nuppu ja valige Käivita. Tippige väljale Ava käsk **regedit** ja seejärel valige OK.

2. Kui teil palutakse lubada registriredaktoril oma seadmes muudatusi teha, valige Jah.

3. Lisage registriredaktoris stringi väärtus **SharedComputerLicensing** sättega 1 jaotises HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. Logige RDS-serveris ***lõppkasutajana*** sisse ja veenduge, et ühisarvuti [aktiveerimine on](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)lubatud Microsoft 365 suurettevõtterakendused .

Lisateavet eeltingimuste, häälestamisjuhiste ja juhiste kohta kohandatud installide kohta leiate Office juurutamistööriista kaudu teemast Microsoft 365 suurettevõtterakendused juurutamine [kaugtöölaua teenuste abil.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Arvuti ühisaktiveerimisega seotud tõrgete lahendamiseks lugege teemat Arvuti ühisaktiveerimisega seotud probleemide [tõrkeotsing Microsoft 365 suurettevõtterakendused](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  