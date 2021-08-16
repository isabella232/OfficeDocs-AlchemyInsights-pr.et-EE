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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028036"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Tõrketeade Microsoft 365 "Kahjuks on teie asutuse teine konto juba sisse logitud".

Probleemi lahendamiseks proovige järgmist.

- Eemaldage kõik töökontod (v.a mõjutatud konto), kasutades Windows Sätted > **Accessi töö- või koolikontot.**
- [Tühjendage Office identimisteabe](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) identimisteabe Windows abil.<br/>
    **Märkus.** 2016. Office registriteed on muutunud 16.0-ks. (Nt: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avage Office'i telefonirakendus Fail   >  **Konto**  >  **Logi välja**. Seejärel logige sisse kehtiva litsentsiga kasutajakontoga. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lisateavet leiate teemast "Kahjuks on teie ettevõtte teine konto selles arvutis juba sisse [logitud", Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)