---
title: Office apps sisselogimisega probleeme
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938191"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Tühi sisselogimiskuva Office'i rakendustes

Selle probleemi lahendamiseks proovige järgmist:
- Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Lähtesta Internet Explorer valikud: valige **Tööriistad** > **Interneti-suvandid** > **Täpsemalt** > **Internet Exploreri sätete lähtestamine** (Pange tähele, et te kaotate kohandatud sätted) ning proovige uuesti sisse logida Office.
- Keelake Windows Defender taotluse valvur (WDAG) või muud sarnast tulemüür või viirusetõrje programmi.
    1. Juhtpaneelil, minge **programmid**ja valige **Windowsi funktsioonide sisse- või väljalülitamine**.
    2. Kui Windows Defender taotluse Guard on lubatud, keelake see.<br/>
    **Märkus:** Peate arvuti taaskäivitama.
- Tagada, et Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ei taotluse või tulemüüri/anti-Anti-Virus programm poolt blokeeritud.
- [Selge Office mandaati](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kasutades Windows Mandaadihaldur.<br/>
    **Märkus:** Registri teed Office 2016 on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Vaadake lisateavet jaotisest [ühenduse küsimusi sisselogimine pärast update Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).