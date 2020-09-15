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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695319"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 rakenduste parandamine "Kahjuks on teie ettevõtte teine konto juba sisse logitud" sõnumis

Probleemi lahendamiseks proovige järgmist.

- Saate eemaldada kõik töökontod (v. a mõjutatud konto), kasutades Windowsi sätteid > **juurdepääs tööle või koolile**.
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.<br/>
    **Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avage Office ' i rakendus, **Valige**  >  **konto**  >  **Logi välja**. Seejärel logige sisse kasutaja kontoga, kellel on kehtiv litsents. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lisateavet leiate teemast ["Kahjuks on teie ettevõtte teine konto juba selles arvutis sisse logitud" Office ' is](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).