---
title: Microsoft 365 rakenduste parandamine, kui teie konto on halvas olekus sõnumis
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744541"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Microsoft 365 rakenduste parandamine "teie konto on halvas olekus" tõrge

Tõrke lahendamiseks proovige probleemses arvutis järgmisi suvandeid.

- Avage Office ' i rakendus, valige suvand **failiserveri**  >  **Account**  >  **Logi kõigist kontodest välja**. Logige uuesti sisse, kasutades kehtiva litsentsiga kasutajakontot. Lisateavet vt teemast [Office’i kontod](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Tühjendage Office ' i mandaat](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows mandaadi halduri abil.<br>
  **Märkus:** Office 2016 registrite teed on muudetud versiooniks 16,0. Näiteks \Software\Microsoft\Office\16.0\Common\Identity\
- Kui Office 365 abil ilmneb tõrge Office ' i 2013 abil, siis lubage Office ' i klientrakenduse jaoks [kaasaegne autentimine](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) .

Lisateavet leiate teemast [rakenduste tõrkeotsing, mis ei saa sisse logida Microsoft 365, Azure ' i või Intune ' i](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

