---
title: Office ' i rakendustele sisselogimisega seotud probleemid
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762982"
---
# <a name="issues-signing-in-to-office-apps"></a>Office ' i rakendustele sisselogimisega seotud probleemid

Office ' i rakendustega sisselogimise probleemide lahendamiseks proovige järgmist.

- Eemaldage kõik töökontod, välja arvatud mõjutatud konto, kasutades Windowsi sätteid > **juurdepääsu töö või kooli**.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , kasutades Windowsi mandaat Manager.<br/>
    **Märkus:** Office 2016 registri teed on muutunud 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avage Office ' i rakendus, valige **faili** > **konto** > **Logi välja**. Seejärel logige sisse, kasutades kehtivat litsentsi kasutajakontoga. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Kui tõrked ilmneb samal ajal, kui ühendate Microsoft 365, kasutades Office 2013, lubage kaasaegne autentimine Office ' i klient.

Lisateavet leiate teemadest
- [Te ei saa sisse logida Microsoft 365, Azure või Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Ühenduse probleemid sisselogimise pärast värskenduse Office 2016 ehitada 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Kahjuks teine konto teie organisatsioonis on juba sisse logitud selles arvutis" Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Sisselogimise probleemide tõrkeotsing Office ' i kaasaegne autentimine ADFS kasutamisel](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)