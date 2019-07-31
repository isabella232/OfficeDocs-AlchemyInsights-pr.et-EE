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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938190"
---
# <a name="issues-signing-in-to-office-apps"></a>Office apps sisselogimisega probleeme

Office apps sisselogimise probleemide lahendamiseks proovige järgmist:

- Eemaldage kõik töö omanikud, välja arvatud mõjutatud konto, kasutades Windowsi sätted > **juurdepääsu tööl või koolis**.
- [Selge Office mandaati](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) kasutades Windows Mandaadihaldur.<br/>
    **Märkus:** Registri teed Office 2016 on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avage mõni Office'i rakendus, valige **faili** > **konto** > **Logi välja**. Seejärel sisse kasutajakontoga, kellel on kehtiv juhiluba. Üksikasjalikuma teabe saamiseks vt [kontode ametisse](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Mac, vaadake [Office 2016 for Mac app ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Vigade ilmnemisel ühendamisel Office 365, Office 2013 kasutades lubada Office'i kliendi kaasaegne autentimise.

Lisateavet vaadake teemast
- [Te ei saa sisse logida Office 365, Azure ja Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Ühenduse probleemid sisselogimine pärast update Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Kahjuks ei õnnestunud teise konto organisatsioonist kirjutatakse juba selles arvutis" asukoht](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Tõrkeotsingu sisselogimiseks Office kaasaegne autentimine kui kasutate ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)