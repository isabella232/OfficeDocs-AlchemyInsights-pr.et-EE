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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938192"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Office'i rakendused "arvuti usaldusväärse platvormi moodul ei tööta korralikult" sõnumi kinnitamine

Probleemi lahendamiseks proovige järgmist:

- Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Selge Office mandaati](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kasutades Windows Mandaadihaldur.<br/>
    **Märkus:** Registri teed Office 2016 on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Proovige [kasutaja taastamise protsess](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) määrata usaldusväärse platvormi mooduli (TPM) ebaõnnestumisi.
- Määra ning EnableADAL = 0, tehes järgmist:  
    1. Paremklõpsake Windowsi nuppu Start, valige **Käivita**, tippige **käsk regedit**ja seejärel klõpsake **nuppu OK**.
    2. Valige **Jah** registriredaktori abil muuta seadme lubamiseks.
    3. Registriredaktoris lisada säte **0** all HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity on **EnableADAL** DWORD-väärtus.

Vaadake lisateavet jaotisest [ühenduse küsimusi sisselogimine pärast update Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).