---
title: RDS Microsoft 365 rakendused terminaliserveris või VDI-s ühiskasutatavad Microsoft 365 rakendused juurutamine
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077246"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS Microsoft 365 rakendused terminaliserveris või VDI-s ühiskasutatavad Microsoft 365 rakendused juurutamine

Kaugtöölaua Microsoft 365 rakendused (RDS) varem terminaliteenuste abil juurutamiseks peate:

- Kui kasutate versiooni Windows (nt Windows 7 SP1, Windows Server 2008 R2), saate kasutada parandust TLS 1.2 vaikeväärtuseks. Hõlpsa lahenduse ja lisateabe saamiseks lugege [teemat TLS 1.1 ja TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)lubamine WinHTTP-s Windows. 
- Teil on leping, mis sisaldab Microsoft 365 suurettevõtterakendused (varem Office 365 Plus). Näiteks Office 365 E3 või Microsoft 365 E5 või mis tahes leping, mis sisaldab Project või Visio töölauaversiooni (nt Project (leping 3) või Visio (leping 2)) või Microsoft 365 Business Premium-plaani, mis sisaldab ka Microsoft 365 ettevõtterakendused.
- Luba arvuti ühisaktiveerimine. Lisateavet leiate teemast Ülevaade arvuti [ühisaktiveerimisest](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)Microsoft 365 rakendused.

**Märkus.** Kui soovite Microsoft 365 rakendused arvuti ühisaktiveerimisrežiimi, laadige alla ja käivitage [Microsoft tugi- ja taasteteenuste abiline](https://aka.ms/SaRA_OfficeSCA_M365Portal). Lisateavet eeltingimuste, häälestusjuhiste ja juhiste kohta installide kohandamiseks Office kohta leiate teemast [Microsoft 365 rakendused juurutamine kaugtöölaua teenuste abil.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Ühisarvuti aktiveerimisega seotud tõrgete lahendamiseks lugege teemat

- [Tõrkeotsing probleemidele, mis on seotud arvuti ühisaktiveerimisega Microsoft 365 rakendused](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Aktiveerimisoleku Microsoft 365 suurettevõtterakendused lähtestamine](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Kui soovite installida Microsoft 365 rakendused RDS-i Microsoft 365 halduskeskus, mis kasutab vaikeinstallisätteid, tehke järgmist.

1. Kontrollige, Microsoft 365 teil on leping. Lisateavet leiate teemast [Mis tellimus mul on?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Vajaduse korral aktiveerige muu Microsoft 365 leping. Lisateavet leiate teemast [Üleminek muule plaanile.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. Kui Microsoft 365 rakendused on RDS-i serverisse installitud mõne muu ühildumatu lepingu abil, desinstallige see, kui **avamiseks valige Juhtpaneel**  >  **Programmi desinstallimine.** Kui teil on probleeme, desinstallige microsoft [tugi- ja taasteteenuste abiline.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. Logige RDS-serveris oma administraatorikontoga sisse Microsoft 365 halduskeskus ja [installige Office](https://portal.office.com/OLS/MySoftware.aspx).

   Pärast Office installimist ärge avage ega logige sisse ühtegi Office rakendusse.

1. Lubage RDS-serveris ühisarvuti aktiveerimine, redigeerides registrit.

   1. Paremklõpsake ekraani Windows vasakus allnurgas olevat nuppu Ja valige **Käivita**. Tippige väljale Ava käsk **regedit** ja seejärel valige **OK**.

   1. Kui teil palutakse lubada registriredaktoril oma seadmes muudatusi teha, valige **Jah**.

   1. Lisage registriredaktori jaotises HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration väärtuse **SharedComputerLicensing** stringiväärtus väärtusega **1** .

1. Logige RDS-serveris lõppkasutajana sisse ja veenduge, et ühisarvuti aktiveerimine on lubatud Microsoft 365 rakendused. 

   Lisateavet leiate teemast [Arvuti ühisaktiveerimise lubamise kontrollimine](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)Microsoft 365 rakendused.