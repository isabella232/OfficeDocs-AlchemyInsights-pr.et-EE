---
title: Parooli tagasikirjutamise lubamine Azure AD Connectis
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
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814008"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Parooli tagasikirjutamise lubamine Azure AD Connectis

Selleks et lubada iseteeninduslikku paroolilähtestuse tagasikirjutamist, peate esmalt Azure AD Connectis lubama tagasikirjutamise võimaluse. Tehke Azure AD Connecti serveri kaudu järgmised toimingud.

1. Logige sisse Azure AD Connecti serverisse ja käivitage **Azure AD Connecti** konfigureerimisviisard.
2. Klõpsake lehel **Tere tulemast** nuppu **Konfigureeri**.
3. Lehel **Lisaülesanded** valige **Kohanda sünkroonimissuvandeid** ja seejärel klõpsake nuppu **Edasi**.
4. Lehel **Loo ühendus Azure AD-ga** sisestage oma Azure’i rentniku üldadministraatori identimisteave ja seejärel klõpsake nuppu **Edasi**.
5. Filtreerimislehtedel **Ühenda kataloogid** ja **Domeen/OÜ** klõpsake nuppu **Edasi**.
6. Lehel **Valikulised funktsioonid** märkige valiku **Parooli tagasikirjutamine** kõrval olev kastike ja klõpsake nuppu **Edasi**.
7. Lehel **Konfigureerimiseks valmis** klõpsake nuppu **Konfigureeri** ja oodake, kuni protsess lõpeb.
8. Kui näete, et konfigureerimine on lõppenud, klõpsake nuppu **Välju**.

Kui parooli tagasikirjutamine on Azure AD Connectis lubatud, konfigureerige Azure AD SSPR-i tagasikirjutamine.  SSPR-is parooli tagasikirjutamise lubamiseks tehke järgmised toimingud.

1. Logige üldadministraatori kontot kasutades sisse Microsoft Azure’i portaali.
2. Otsige üles **Azure Active Directory** ja valige see, klõpsake valikut **Paroolilähtestus** ning seejärel valikut **Kohapealne integreerimine**.
3. Määrake küsimuse **Soovite paroole tagasi kirjutada oma kohapealsesse kataloogi?** vastuseks **Jah**.
4. Määrake küsimuse **Lubate kasutajatel kontosid lukust avada ilma oma parooli lähtestamata?** vastuseks **Jah**.
5. Kui olete valmis, klõpsake nuppu **Salvesta**.

Lisateavet leiate artiklist [Kuidas lubada Azure Active Directoryil iseteeninduslikku paroolilähtestuse tagasikirjutamist kohapealsesse keskkonda](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Kui administraator lähtestab Azure’i portaalis kasutaja parooli ja see on väliskasutaja või parool räsisünkroonitud, kirjutatakse parool tagasi kohapealsesse keskkonda. See funktsioon nõuab Azure’i Premium-litsentsi (P1 või P2) ja hetkel pole see Office’i haldusportaalis toetatud.
