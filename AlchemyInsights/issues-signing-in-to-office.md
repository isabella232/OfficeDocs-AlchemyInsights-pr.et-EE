---
title: Microsoft 365 rakendustesse sisselogimisega seotud probleemid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695283"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tühi sisselogimiskuva Microsoft 365 rakendustes

Probleemi lahendamiseks proovige teha järgmist.
- Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office '](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile.
- Internet Exploreri suvandite lähtestamine: valige **Tööriistad**  >  **Interneti-suvandid**  >  **täiustatud**  >  **lähtestage Internet Exploreri sätted** (Pange tähele, et te kaotate kohandatud sätted) ja proovige siis uuesti Office ' isse sisse logida.
- Keelake Windows Defender Application Guard (WDAG) või mõni muu sarnane tulemüür või viirusetõrje programm.
    1. Avage juhtpaneelil jaotis **programmid**ja seejärel valige Windowsi funktsioonide sisse- **või väljalülitamine**.
    2. Kui Windows Defenderi rakenduse valvur on lubatud, proovige see keelata.<br/>
    **Märkus:** Võimalik, et peate arvuti taaskäivitama.
- Veenduge, et rakenduse või tulemüüri/viirusetõrje programm ei blokeeriks Microsoft. AAD. BrokerPlugin [AAD WAM lisandmoodulit](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) .
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.<br/>
    **Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisateavet leiate teemast [probleemid seoses sisselogimisega pärast Windows 10 versioonile Office 2016 Build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).