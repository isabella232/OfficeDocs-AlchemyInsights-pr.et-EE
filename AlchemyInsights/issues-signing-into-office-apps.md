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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695175"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 rakenduste parandamine teie arvuti usaldusväärse platvormi moodul ei tööta õigesti "sõnum

Probleemi lahendamiseks proovige järgmist.

- Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office '](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.<br/>
    **Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Proovige lahendada usaldusväärse platvormi mooduli (TPM) tõrked [kasutaja taastamise protsessis](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .
- Seadke EnableADAL = 0, kasutades järgmisi juhiseid.  
    1. Paremklõpsake Windowsi nuppu Start, valige käsk **Käivita**, tippige **käsk regedit**ja seejärel klõpsake nuppu **OK**.
    2. Kui soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige **Jah** .
    3. Registriredaktori korral lisage **ENABLEADAL** DWORD-väärtus, mille sätteks **on HKEY_CURRENT_USER** \software\microsoft\office\16.0\common\identity.

Lisateavet leiate teemast [probleemid seoses sisselogimisega pärast Windows 10 versioonile Office 2016 Build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).