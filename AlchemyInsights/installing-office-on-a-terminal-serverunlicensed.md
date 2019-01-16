---
title: Paigaldus office Terminal Server - litsentseerimata
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28285728"
---
# <a name="installing-office-on-a-terminal-server"></a>Paigaldus Office terminali Server

Kohta Office 365 ProPlusi kasutades kaugtöölaua teenuste (RDS) server Windowsi, endise nimega terminaliteenused:
  
- Peab teil olema Office 365 leping, mis sisaldab Office 365 ProPlus, Office 365 Enterprise E3 või Enterprise E5. Office 365 Business ja Office 365 Business Premium lepingute ei sisalda Office 365 ProPlus.
    
- Peate lubama [ühiskasutatavas arvutis aktiveerimisega](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Kui soovite installida Office 365 ProPlus RDS portaalist Office 365, ** *mis kasutab vaikimisi installimise sätted* **, järgige neid samme: 
  
1. Vaata mida teil Office 365 leping. [Õpi kuidas](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Kui lüliti erinevate Office 365 korral. [Õpi kuidas](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Kui Office on juba installitud, kasutades Office 365 lepingud RDS server, eemaldage see. Näiteks minnes juhtpaneelil \> programmi desinstallimine. Desinstallige [Microsoft Support ja taastamise abimees](https://aka.ms/SARA-OfficeUninstall-Alchemy) kui teil tekib küsimusi. 
    
4. RDS server, logige sisse Office 365 portaali administraatori kontoga ja [installige Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Pärast Office'i installimist ** *Ärge avage või logige sisse* ** et kõik Office'i rakendused. 
    
6. RDS server, luba ühiskasutatavas arvutis aktiveerimisega redigeerige registrit järgmiselt:
    
1. Ekraani alumises vasakus nurgas nuppu Windows paremklõpsake ja valige käsk Käivita. Väljale Ava **tippigeregedit**, ja seejärel klõpsake nuppu OK. 
    
2. Valige Jah kui teil palutakse Registry Editor võimaldab muuta seadme.
    
3. Registry Editor, lisage string väärtus **SharedComputerLicensing** säte on HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration 1. 
    
7. RDS server ** *lõppkasutajad sisselogimise* ** ja [ühiskasutatavas arvutis aktiveerimisega on lubatud jaoks Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Eeltingimused, juhiseid ja suuniseid kohandatud installide kasutate Office'i juurutamise tööriist üksikasjalikumalt, vt [Juurutamine Office 365 ProPlusi kasutades kaugtöölaua teenused](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Ühiskasutatavas arvutis aktiveerimisega seotud tõrgete lahendamiseks vaadake [tõrkeotsing küsimusi ühiskasutatavas arvutis aktiveerimisega jaoks Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

