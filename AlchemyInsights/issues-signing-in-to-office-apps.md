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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833071"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 rakenduste parandamine sõnum "Kahjuks on teie asutuse teine konto juba sisse logitud".

Probleemi lahendamiseks proovige järgmist.

- Eemaldage kõik töökontod (v.a mõjutatud konto), kasutades Windowsi > **Accessi töö- või koolisätteid.**
- [Tühjendage Windowsi identimisteabe](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) halduri abil Office'i identimisteavet.<br/>
    **Märkus.** Office 2016 registriteed on muutunud 16.0-ks. (Nt: \Software\Microsoft\Office\16.0\Common\Identity\)
- Avage Office'i rakendus ja valige **Fail**  >  **Konto**  >  **logi välja**. Seejärel logige sisse kehtiva litsentsiga kasutajakontoga. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Maci kasutajad võiksid lugeda artiklit [Office 2016 for Maci rakendusse ei saa sisse logida](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Lisateavet leiate Office'is teemast "Kahjuks on teie ettevõtte teine konto selles arvutis juba sisse [logitud".](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)