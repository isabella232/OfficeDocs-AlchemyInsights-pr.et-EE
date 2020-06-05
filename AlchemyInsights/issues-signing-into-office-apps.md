---
title: Probleemid sisselogimisel Microsoft 365 rakendused
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579861"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 rakenduste kinnitamine "teie arvuti usaldusväärse platvormi moodul ei tööta korralikult" sõnum

Probleemi lahendamiseks proovige järgmist.

- Installige uusimad värskendused [Windowsi](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office ' i](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)jaoks.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.<br/>
    **Märkus:** Office 2016 registri teed on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Proovige [kasutaja taasteprotsessi](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) usaldusväärse platvormi MOODULI (TPM) tõrgete lahendamiseks.
- Seadke EnableADAL = 0, kasutades järgmisi samme:  
    1. Paremklõpsake Windowsi Start nuppu, valige **Käivita**, tippige **käsk regedit**ja seejärel valige **OK**.
    2. Valige **Jah** , et lubada registriredaktoris teie seadmes muudatusi teha.
    3. Registry Editoris lisada DWORD-väärtus **Enableadal** sätte **0** all HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.

Lisateabe saamiseks vaadake [ühenduse probleemid sisse logida pärast värskenduse Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).