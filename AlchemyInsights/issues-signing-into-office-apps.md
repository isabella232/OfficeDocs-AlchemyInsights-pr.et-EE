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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709102"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 rakenduste parandamine teie arvuti usaldusväärse platvormi moodul ei tööta õigesti "sõnum

Probleemi lahendamiseks proovige järgmist.

- Installige uusimad värskendused [Windowsile](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office '](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)ile.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.<br/>
    **Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Proovige lahendada usaldusväärse platvormi mooduli (TPM) tõrked [kasutaja taastamise protsessis](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .
- Seadke EnableADAL = 0, kasutades järgmisi juhiseid.  
    1. Paremklõpsake Windowsi nuppu Start, valige käsk **Käivita**, tippige **käsk regedit** ja seejärel klõpsake nuppu **OK**.
    2. Kui soovite, et registriredaktori saaks teie seadmes muudatusi teha, valige **Jah** .
    3. Registriredaktori korral lisage **ENABLEADAL** DWORD-väärtus, mille sätteks on **0** jaotises HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Lisateavet leiate teemast [probleemid seoses sisselogimisega pärast Windows 10 versioonile Office 2016 Build 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).