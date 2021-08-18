---
title: Probleemid sisselogimisel Microsoft 365 rakendustesse
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088032"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Tühi sisselogimiskuva Microsoft 365 rakendustes

Selle probleemi lahendamiseks proovige järgmist.
- Installige uusimad värskendused [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [ja Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Internet Exploreri suvandite lähtestamine. Avage **Tööriistad**  >  **Internet Options**  >  **Advanced** Reset Internet Explorer Sätted (pange tähele, et kaotate kohandatud sätted) ja proovige uuesti  >   Office sisse.
- Keelake Windows Defender Application Guard (WDAG) või muu sarnane tulemüür või viirusetõrjeprogramm.
    1. Valige juhtpaneelil Programmid ja **seejärel** käsk Lülita Windows **sisse või välja**.
    2. Kui Windows Defender Application Guard on lubatud, proovige see keelata.<br/>
    **Märkus.** Võimalik, et peate arvuti taaskäivitama.
- Veenduge, et ükski rakendus ega tulemüür/viirusetõrjeprogramm ei blokeeriks [AAD WAM-lisandmoodulit Microsoft.AAD.BrokerPlugin AAD WAM.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)
- [Tühjendage Office identimisteabe](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) identimisteabe Windows abil.<br/>
    **Märkus.** 2016. Office registriteed on muutunud 16.0-ks. (Nt: \Software\Microsoft\Office\16.0\Common\Identity\)

Lisateavet leiate teemast Ühenduseprobleemid sisselogimisel pärast Office [2016. aasta järku 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).