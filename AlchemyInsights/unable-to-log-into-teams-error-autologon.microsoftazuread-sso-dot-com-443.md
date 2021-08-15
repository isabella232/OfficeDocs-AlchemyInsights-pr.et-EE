---
title: Tõrke autologon.microsoftazuread-sso.com:443 tõttu ei saa Teamsi sisse logida
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038396"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Tõrke autologon.microsoftazuread-sso dot com:443 tõttu ei saa Teamsi sisse logida

Kui O365 autentimisena on lubatud sujuv SSO, võib sisevõrgu saitide jaoks olla vajalik lisada URL „autologon.microsoftazuread-sso.com“.  Kui see on eelnevalt lisatud usaldusväärsete saitide hulka ja kasutusel on sujuv SSO, tuleks see usaldusväärsete saitide seast eemaldada.

Vaadake teemat [Tõrgeteta SSO tõrkeotsingu kontroll-loend](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

URL-i sisevõrgu saitide loendisse lisamieks järgige järgmisi samme.

1. Avage Internet Explorer, klõpsates nuppu **Start**. Tippige otsinguväljale Internet Explorer ja seejärel klõpsake tulemite loendis valikut **Internet Explorer**.
2. Klõpsake nuppu **Tööriistad** ja seejärel klõpsake valikut **Interneti-suvandid**.
3. Klõpsake vahekaarti **Turvalisus**.
4. Nüüd klõpsake suvandit **Kohaliku sisevõrgu saidid** ja seejärel klõpsake **saitide** nuppu ja seejärel nuppu **Täpsemalt**.
5. Sisestage veebisaidi URL ja klõpsake suvandit **Lisa**.
6. Kui olete lõpetanud, klõpsake suvandit **Sulge**.

Lisateavet leiate teemast [O365 sujuva SSO juurutamise dokumentatsioon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (sh poliitikal põhinev protsess, mis lisab 3. juhises sisevõrgu saitidele URL-i).
