---
title: Microsoft 365 rakendustesse sisselogimisega seotud probleemid
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833027"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tühi sisselogimiskuva Microsoft 365 rakendustes

Selle probleemi lahendamiseks proovige järgmist.
- Installige Windowsi ja [Office'i uusimad](https://support.microsoft.com/help/4027667/windows-10-update) [värskendused.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Internet Exploreri suvandite lähtestamine: avage **Tööriistad** Interneti-suvandid Internet Exploreri sätete täpsem lähtestamine (arvestage, et kaotate kohandatud sätted) ja proovige uuesti  >    >    >   Office'i sisse logida.
- Keelake Windows Defenderi rakendusekaitse (WDAG) või muu sarnane tulemüür või viirusetõrjeprogramm.
    1. Avage juhtpaneelil Programmid ja **seejärel** valige Lülita Windowsi funktsioonid sisse **või välja.**
    2. Kui Windows Defenderi rakendusekaitse on lubatud, proovige see keelata.<br/>
    **Märkus.** Võimalik, et peate arvuti taaskäivitama.
- Veenduge, et ükski rakendus ega tulemüür/viirusetõrjeprogramm ei blokeeriks [AAD WAM-lisandmoodulit Microsoft.AAD.BrokerPlugin AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Tühjendage Windowsi identimisteabe](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) halduri abil Office'i identimisteavet.<br/>
    **Märkus.** Office 2016 registriteed on muutunud 16.0-ks. (Nt: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisateavet leiate teemast Ühenduseprobleemid sisselogimisel pärast [windows 10 opsüsteemis Office 2016 järgule 16.0.7967 värskendamist.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)