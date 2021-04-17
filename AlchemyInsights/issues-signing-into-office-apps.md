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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832999"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 rakenduste parandamine teade "Teie arvuti usaldusväärse platvormi moodul ei tööta õigesti".

Probleemi lahendamiseks proovige järgmist.

- Installige Windowsi ja [Office'i uusimad](https://support.microsoft.com/help/4027667/windows-10-update) [värskendused.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Tühjendage Windowsi identimisteabe](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) halduri abil Office'i identimisteavet.<br/>
    **Märkus.** Office 2016 registriteed on muutunud 16.0-ks. (Nt: \Software\Microsoft\Office\16.0\Common\Identity\)
- Proovige [kasutajataasteprotsessi usaldusväärse](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) platvormi mooduli (TPM) tõrgete lahendamiseks.
- Määrake EnableADAL = 0 järgmiste juhiste abil.  
    1. Paremklõpsake Windowsi nuppu Start, valige **Käivita**, tippige **käsk regedit** ja seejärel valige **OK**.
    2. Valige **Jah,** et registriredaktor lubaks teie seadmes muudatusi teha.
    3. Lisage registriredaktoris **EnableADAL-i** DWORD-väärtus sättega **0** jaotises HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisateavet leiate teemast Ühenduseprobleemid sisselogimisel pärast [windows 10 opsüsteemis Office 2016 järgule 16.0.7967 värskendamist.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)