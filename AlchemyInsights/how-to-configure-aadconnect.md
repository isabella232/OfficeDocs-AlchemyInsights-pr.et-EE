---
title: 646 kuidas konfigureerida AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722531"
---
# <a name="configure-sync-features"></a>Sünkroonimise funktsioonide konfigureerimine

Azure AD ühenduse sisaldab mitmeid funktsioone, mis on vaikimisi lubatud või et saate lubada hiljem. Mõned funktsioonid vajavad täiendavat konfiguratsiooni konkreetses keskkonnas.

- [Filtreerimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) piirab objektid SÜNKROONITAKSE Azure AD. Vaikimisi sünkroonitakse kõik kasutajad, kontaktid, rühmad ja Windows 10 arvutikontod. Saate objekte lisada või välistada domeenide, organisatsiooniüksused või muude atribuutide alusel.

- [Parooli Hash sünkroonimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sünkroonib parooli Hash asutusesisese Active DIRECTORY Azure AD. See võimaldab parooli haldamine ühes kohas, kuid sama parooli kasutamine nii asutusesisese kui ka pilve keskkondades. Kuna Active Directory on autoriteetne allikas, saate kasutada oma paroolipoliitikat.

- [Iseteeninduse parooli lähtestamine (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) võimaldab kasutajatel lähtestada oma paroolid pilve samas endiselt rakendada oma asutusesisese parooli poliitika.

- [Seadme tagasikirja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) võimaldab registreeritud seadmete Azure AD kirjutatakse tagasi asutusesisese Active Directory, et neid saab kasutada tingimuslik juurdepääs.

- [Vältida juhuslikku kustutamist](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on vaikimisi lubatud, et aidata vältida liiga palju samaaegseid objekti kustutamist (rohkem kui 500 objektid sünkroonimise kohta). Seda sätet saate muuta oma organisatsiooni vajaduste rahuldamiseks.

- [Automaatne täiendamine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on vaikimisi lubatud Express seadmete jaoks ja aitab tagada, et teie Azure AD ühenduse versioon on alati praegune.
