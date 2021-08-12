---
title: 646 AADConnecti konfigureerimine
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963639"
---
# <a name="configure-sync-features"></a>Sünkroonimisfunktsiooni konfigureerimine

Azure AD Ühendus sisaldab mitut funktsiooni, mis on vaikimisi lubatud või mille saate hiljem lubada. Mõnede funktsioonide jaoks on vaja teatud keskkondades täiendavat konfigureerimist.

- [Filtreerimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) piirab objektide sünkroonimist Azure AD-ga. Vaikimisi sünkroonitakse kõik kasutajad, kontaktid, rühmad Windows 10 kontod. Objekte saate kaasata või välistada domeenide, OU-de või muude atribuutide põhjal.

- [Paroolisortsünkroonimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sünkroonib paroolisort asutusesiseseSt Active Directoryst Azure AD-ga. See võimaldab paroolihaldust ühes kohas, kuid sama parooli saab kasutada nii kohapeal kui ka pilvekeskkonnas. Kuna Active Directory on autoriteetne allikas, saate kasutada oma paroolipoliitikaid.

- [Iseteeninduse parooli lähtestamine (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) võimaldab kasutajatel lähtestada oma paroolid pilveteenuses, rakendades samal ajal teie kohapealse paroolipoliitika.

- [Seadme tagasikirjutus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) võimaldab Azure AD registreeritud seadmetel uuesti asutusesisesesse Active Directorysse kirjutada, et neid saaks kasutada tingimusjuurdepääsuks.

- [Juhuslike kustutamiste](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) keelamine on vaikimisi lubatud, et vältida liiga palju samaaegseid objektide kustutamist (üle 500 objekti sünkroonimise kohta). Seda sätet saate muuta vastavalt oma asutuse vajadustele.

- [Automaatne versioonitäiendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on kiirinstallide korral vaikimisi lubatud ja see aitab tagada, et teie Azure AD Ühendus oleks alati ajas.
