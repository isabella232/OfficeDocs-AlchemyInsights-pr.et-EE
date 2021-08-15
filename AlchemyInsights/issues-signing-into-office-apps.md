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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986887"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Tõrketeade Microsoft 365 "Teie arvuti usaldusväärse platvormi moodul ei tööta õigesti" parandamine

Probleemi lahendamiseks proovige järgmist.

- Installige uusimad värskendused [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [ja Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Tühjendage Office identimisteabe](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) identimisteabe Windows abil.<br/>
    **Märkus.** 2016. Office registriteed on muutunud 16.0-ks. (Nt: \Software\Microsoft\Office\16.0\Common\Identity\)
- Proovige [kasutajataasteprotsessi usaldusväärse](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) platvormi mooduli (TPM) tõrgete lahendamiseks.
- Määrake EnableADAL = 0 järgmiste juhiste abil.  
    1. Paremklõpsake nuppu Windows Start, valige **Käivita**, tippige **käsk regedit** ja seejärel valige **OK**.
    2. Valige **Jah,** et registriredaktor lubaks teie seadmes muudatusi teha.
    3. Lisage registriredaktoris **EnableADAL-i** DWORD-väärtus sättega **0** jaotises HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisateavet leiate teemast Ühenduseprobleemid sisselogimisel pärast Office [2016. aasta järku 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).