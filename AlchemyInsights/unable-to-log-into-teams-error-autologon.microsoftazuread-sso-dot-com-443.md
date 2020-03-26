---
title: Tõrke autologon.microsoftazuread-sso.com:443 tõttu ei saa Teamsi sisse logida
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931902"
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
