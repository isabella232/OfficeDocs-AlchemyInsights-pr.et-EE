---
title: Parooli sünkroonimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960831"
---
# <a name="password-synchronization"></a>Parooli sünkroonimine

**Parooliga hashisünkroonimine ei tööta üldse**

Levinumad probleemid, mis ilmnevad klientidel, kui paroolisahisünkroonimine ei tööta, on järgmised.

- Active Directory kontole, mida Azure AD Ühendus kasutab asutusesisese Active Directoryga  suhtlemiseks,  ei anta paljundamiskataloogi muudatusi ega paljunda kataloogi muudatusi Kõik õigused, mis on vajalikud paroolisünkroonimiseks – peate selle lahendama, andes need õigused Active Directory kontole.
- Paroolisorni sünkroonimine keelatakse pärast seda, kui  administraator on muutnud kasutaja Sign-In-meetodi paroolisünkroonimiseks mõneks muuks suvandiks (nt Azure  AD Ühendus viisardis **AD FS-iga FS-iga** liitumine) – probleemi lahendamiseks lubate Azure AD Ühendus viisardis uuesti paroolisorgisünkroonimise funktsiooni.
- Ühenduvusprobleem asutusesisese Active Directoryga. Näiteks azure AD Ühendus ei pääse mõnedele domeenikontrolleritele [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) juurde või nõutavad pordid on tulemüüri poolt blokeeritud. Selle probleemi lahendamiseks peate tagama Azure AD Ühendus serveri ja asutusesisese Active Directory vahelise ühenduvuse.
- Azure AD Ühendus server on praegu staging režiimis, mille tulemusena server ei saa parooliga seotud hashes - Probleemi tõrkeotsinguks järgige teemas Parooli sünkroonimise tõrkeotsing [Azure AD Ühendus sünkroonimist –](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)paroole ei sünkroonita.

**Parooliga hashisünkroonimine ei tööta mõnede kasutajate jaoks**

1. Kui märkasite, et kasutaja paroolisort ei  sünkroonita, kasutage probleemi uurimiseks ja lahendamiseks Azure AD Ühendus tõrkeotsinguülesannet. Tehke järgmised toimingud.

    a. [Tõrkeotsinguülesande käivitamine viisardis](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Tõrkeotsingu cmdlet-käsu abil saate uurida parooliga sünkroonimise probleemi konkreetses kasutuses](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Kohapealne Active Directory kasutajaobjekt on lubatud, kui **kasutaja peab järgmisel sisselogimisel parooli** muutma. Kui see suvand on lubatud, määratakse kasutajale ajutine parool ja kasutajal palutakse järgmisel sisselogimisel parooli muuta. Azure AD Ühendus sünkroonida ajutisi paroole Azure AD-ga.

Ülaltoodud probleemi lahendamiseks tehke ühte järgmistest toimingutest.

- Paluge kasutajal sisse logida asutusesisesesse rakendusse (nt Windows Desktop) ja muuta parooli. Uus parool sünkroonitakse Azure AD-ga.
- Kui administraator värskendab kasutaja parooli, ilma et lubaks suvandit **Kasutaja** peab järgmisel sisselogimisel parooli muutma, ja jagage uut parooli kasutajaga.

3. Kohapealne Active Directory kasutajaobjekt pole **objektisünkroonimise või** paroolisünkroonimise jaoks õigesti konfigureeritud. Selle probleemi tõrkeotsinguks järgige juhiseid, mida on kirjeldatud teemas Paroolisiga sünkroonimise tõrkeotsing [Azure AD Ühendus sünkroonimist.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







