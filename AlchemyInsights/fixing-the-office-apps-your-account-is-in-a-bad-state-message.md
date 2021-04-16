---
title: Microsoft 365 rakenduste parandamine Teie kontol on halb olekuteade
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812532"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365 rakenduste vea "Teie konto on halvas olekus" parandamine

Selle tõrke lahendamiseks proovige mõjutatud arvutis järgmisi suvandeid.

- Avage Office'i rakendus, valige **Fail**  >  **Konto**  >  **Logi välja kõigilt kontodelt.** Logige uuesti sisse kehtiva litsentsiga kasutajakontoga. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Tühjendage Windowsi identimisteabe](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) halduri abil Office'i identimisteavet.<br>
  **Märkus.** Office 2016 registriteed on muutunud 16.0-ks. Näiteks \Software\Microsoft\Office\16.0\Common\Identity\
- Kui Office 365-ga Office 2013 ühenduse loomisel ilmneb tõrge, lubage Office'i [klientrakenduse](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) jaoks modernautentimine.

Lisateavet leiate teemast Microsoft [365, Azure'i või Intune'i](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)mitte-brauserirakenduste tõrkeotsing.

