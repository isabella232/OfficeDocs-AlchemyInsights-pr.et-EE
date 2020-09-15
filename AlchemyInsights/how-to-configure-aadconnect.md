---
title: 646 Aadconnecti konfigureerimine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704485"
---
# <a name="configure-sync-features"></a>Sünkroonimise funktsioonide konfigureerimine

Azure AD Connect sisaldab mitmeid funktsioone, mis on vaikimisi lubatud või mida saate hiljem lubada. Mõned funktsioonid vajavad teatud keskkondades täiendavat konfiguratsiooni.

- [Filtreerimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) piirab objektide sünkroonimist Azure AD-ga. Vaikimisi sünkroonitakse kõik kasutajad, kontaktid, rühmad ja Windows 10 arvuti kontod. Saate objekte lisada või välistada domeenide, objektide või muude atribuutide põhjal.

- [Parool Hash sünkroonimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sünkroonib parool Hash kohapealse Active DIRECTORY Azure AD. See lubab ühes kohas kasutada parooli, kuid sama parooli kasutamine nii kohapealses kui ka pilveteenuse keskkonnas. Kuna Active Directory on autoriteetne allikas, saate kasutada oma parooli poliitikaid.

- [Iseteeninduskeskuse parooli lähtestamine (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) võimaldab kasutajatel oma paroole pilve lähtestada, rakendades samal ajal ka kohapealset parooli poliitikat.

- [Seadme tagasikirjutusega](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) võimaldab Azure AD registreeritud seadmetel kirjutada tagasi kohapealsesse Active Directorys, et neid saaks kasutada tingimusjuurdepääsu jaoks.

- [Juhuslike kustutamise vältimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on vaikimisi lubatud, et vältida liiga palju üheaegsete objektide kustutamist (rohkem kui 500 objekti sünkroonimise kohta). Seda seadet saate muuta oma asutuse vajaduste täitmiseks.

- [Automaatne täiendamine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on vaikimisi lubatud, sest see on mõeldud vaikimisi ja aitab tagada, et teie Azure AD Connecti versioon on alati aktiivne.
