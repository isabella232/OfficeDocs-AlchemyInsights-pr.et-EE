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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481445"
---
# <a name="password-synchronization"></a>Parooli sünkroonimine

**Parooli Hash sünkroonimine ei tööta üldse**

Mõned levinud probleemid klientidega, kui parooli Hash sünkroonimine ei tööta, on järgmised.

- Azure AD ' is kasutatava Active Directory kontoga suhtlemiseks kohapealse Active Directory abil pole antud **tiražeerimise kataloogi muudatusi** ja **tiražeerimise register muudab kõik** juurdepääsuõigused, mida on vaja parooli sünkroonimiseks – peate selle parandama, andes need juurdepääsuõigused Active Directory kontole.
- Parooli Hash sünkroonimine on keelatud pärast seda, kui administraator muutis kasutaja Sign-In meetod **parooli sünkroonimise** teise variandi (nt **Föderatsioon AD FS** Azure AD Connecti viisardiga) – saate selle parandada, kui lubate Azure AD Connecti viisardis **parooli Hash sünkroonimise** funktsiooni.
- Ühenduvuse probleem kohapealne Active Directoryga. Näiteks ei pääse mõned domeenikontrollerid Azure AD Connecti kaudu juurde või tulemüürid [on blokeeritud](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) , peate selle parandama, tagades, et Azure AD Connecti serveri ja kohapealse Active Directory vaheline Ühenduvus töötab õigesti.
- Azure AD Connect server on praegu lavastuse režiimis, mille tulemusena server ei saa parooli hashes-probleemi tõrkeotsinguks, järgige jaotises kirjeldatud juhiseid, mida on kirjeldatud jaotises [tõrkeotsing parooliga sünkroonimisel AZURE ad Connecti sünkroonimine – paroole ei sünkroonita](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Parooli Hash sünkroonimine ei tööta mõne kasutaja jaoks**

1. Kui märkate, et parooli Hash ei sünkroonita kasutaja jaoks, kasutage probleemi uurimiseks ja lahendamiseks Azure AD ' i ülesande **tõrkeotsingut** . Tehke järgmised toimingud.

    loomine. [Viisardis tõrkeotsingu ülesande käivitamine](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Tõrkeotsingu cmdlet-käsu kasutamine konkreetsel otstarbel parooli räsi sünkroonimise probleemi uurimiseks](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Kohapealne Active Directory User Object on lubatud **kasutaja peab parooli muutma järgmisel sisselogimise** suvandil. Kui see suvand on lubatud, määratakse kasutajale ajutine parool ja teil palutakse muuta järgmise sisselogimise parooli. Azure AD Connecti ei sünkroonita Azure AD ajutised paroolid.

Ülaltoodud probleemi lahendamiseks tehke ühte järgmistest toimingutest.

- Paluge kasutajal sisse logida asutusesisesesse rakendusse (nt Windowsi töölauale) ja muuta parooli. Uus parool sünkroonitakse Azure AD-ga.
- Kui administraator on kasutaja parooli värskendanud, siis peab kasutaja parooli **muutma järgmisel sisselogimisel parooli vahetama** ja kasutajaga uue parooli ühiskasutusse andma.

3. Kohapealne Active Directory kasutaja objekt pole objekti sünkroonimiseks või parooli sünkroonimiseks **õigesti konfigureeritud** . Selle probleemi tõrkeotsingu sooritamiseks järgige juhiseid, mis on kirjeldatud jaotises [tõrkeotsing parooli räsi sünkroonimisel AZURE ad Connecti sünkroonimine](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







