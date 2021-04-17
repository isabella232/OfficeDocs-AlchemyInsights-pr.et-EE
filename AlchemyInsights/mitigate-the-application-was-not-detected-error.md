---
title: Tõrke Rakendust ei leitud lahendamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836347"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Tõrke „Rakendust ei leitud“ lahendamine

Intune’i edastatud rakenduse installimise tõrge „Rakendust ei leitud pärast installimise edukat lõpuleviimist“ võib ilmneda kõigil peamistel OS-i platvormidel (Windows, iOS ja Android).

Levinumad seda tõrget tekitavad stsenaariumid on järgmised.

- Pärast algset juurutamist värskendati rakendus väljaspool Intune’i (kolmanda osapoole rakenduste poest). Näiteks võivad osad rakendused (nt Google Chrome) teha automaatseid värskendusi.
- Kasutaja on rakenduse pärast esialgset installimist desinstallinud.

Selle probleemi lahendamiseks kõigepealt vaadake mõjutatud seadmed läbi et teha kindlaks tõrke ilmnemise stsenaarium.

- Kui rakendust värskendati väljaspool Intune’i, saab rakenduse käivitamise häälestada rakenduse versiooni ignoreerima. Selleks määrake jaotises **Rakenduse konfigureerimine > Rakenduse teave** suvand **Ignoreeri rakendust** valikule **Jah**.
- Sihtklientide jaoks võib olla asjakohane juurutada rakenduse „nagu vaja“ ja tagada, et juurutatud oleks uusim versioon.
- Teise võimalusena on iOS-i platvormil võimalik kasutada funktsiooni **automaatne uuendamine**, mis on seostatud Apple’i mahu ostmise programmiga, mille saab konfigureerida automaatselt värskendama uuele versioonile, kui need avaldatakse.

Rakenduse installiprobleemide tõrkeotsingu kohta leiate lisateavet teemast [Rakenduse installiprobleemide tõrkeotsing](https://docs.microsoft.com/intune/troubleshoot-app-install).
