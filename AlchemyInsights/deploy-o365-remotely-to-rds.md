---
title: Microsoft 365 rakenduste juurutamine rakenduses RDS, terminaliserveri või VDI ühiskasutusse antud rakenduse Enterprise jaoks
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786273"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365 rakenduste juurutamine rakenduses RDS, terminaliserveri või VDI ühiskasutusse antud rakenduse Enterprise jaoks

Microsoft 365 rakenduste juurutamiseks kaugtöölaua teenuste (RDS), varem nimega terminaliteenuste abil, tehke järgmist.
- Teil peab olema Microsoft 365 äriplaani või Office 365 lepingu jaoks, mis sisaldab Microsoft 365 Enterprise ' i jaoks mõeldud rakendusi (nt Office 365 Enterprise E3 või Enterprise E5).
   > [!NOTE] 
   > Microsoft 365 Apps for Business ja Microsoft 365 Business Premium Standard lepingud ei sisalda Microsoft 365 Apps for Enterprise.
- Peate lubama [ühiskasutatava arvuti aktiveerimise](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Samuti saate alla laadida ja käivitada [Microsofti tugiteenuste ja taastekonsooli abilise](https://aka.ms/SaRA_OfficeSCA_M365Portal) , et installida Office ' i ühiskasutusega arvuti aktiveerimise režiimis Microsoft 365 rakendused.

Lisateavet Office ' i juurutamise tööriista kasutamise eeltingimuste, häälestamise juhiste ja kohandatud installide kohta leiate teemast [microsofti 365 rakenduste juurutamine kaugtöölaua teenuste abil](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Ühiskasutusega arvuti aktiveerimisega seotud tõrgete lahendamiseks tehke järgmist.
- Lugege teemat [Office ' i jaoks mõeldud Microsoft 365 rakenduste ühiskasutusega arvuti aktiveerimisega seotud probleemide tõrkeotsing](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Lugege artiklit [Microsoft 365 suurettevõtterakenduste aktiveerimisoleku lähtestamine](https://go.microsoft.com/fwlink/?linkid=2109218) (inglise keeles).

Kui soovite installida Microsoft 365 rakendusi RDS-ile Microsoft 365 halduskeskus, ***mis kasutab vaikimisi installi sätteid***, tehke järgmist.

1.    Vaadake, milline tellimus teil on. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Vajadusel aktiveerige mõni muu pakett. [Vaadake, kuidas](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Kui Office on juba RDS-serverisse installitud mis tahes muu Microsofti tellimuse kaudu, desinstallige see. Näiteks **juhtpaneeli**käsuga  >  **Desinstalli programm**. Kui teil on probleeme, desinstallige [Microsoft support ja Recovery Assistanti](https://aka.ms/SARA-OfficeUninstall-Alchemy) abil.
4.    Rakenduses RDS logige sisse oma administraatori kontoga Microsoft 365 halduskeskus ja [installige Enterprise ' i jaoks microsoft 365](https://portal.office.com/OLS/MySoftware.aspx)' i rakendused.
5.    Kui Office on installitud, ***Ärge avage ega logige sisse*** ühtegi Office ' i rakendusse.
6.    RDS-serveris lubage ühiskasutusega arvuti aktiveerimine, redigeerides registrit, järgides järgmisi juhiseid.
   1. Paremklõpsake Kuva vasakus allnurgas nuppu Windows ja valige **Käivita**. Tippige väljale Ava **käsk regedit**ja seejärel klõpsake **nuppu OK**.
   2. Kui teilt küsitakse, kas soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige **Jah** .
   3. Lisage registriredaktori **SharedComputerLicensing** stringi väärtus, mille sätteks on HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. RDS-serveris ***logige sisse lõppkasutajana*** ja veenduge, [et ühiskasutusega arvuti aktiveerimine oleks lubatud Microsoft 365 rakenduste jaoks Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)' i jaoks.

