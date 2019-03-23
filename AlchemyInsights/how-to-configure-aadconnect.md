---
title: 646 kuidas seadistada AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779508"
---
# <a name="configure-sync-features"></a>Sünkroonimise funktsioonide konfigureerimine

Azure AD ühenduse loomine hõlmab funktsioone, mis on vaikimisi või saate lubada hiljem. Mõni nõuda täiendavaid konfiguratsiooni teatud keskkondades.
  
- [Filtreerimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) piirid objektid on sünkroonitud Azure AD. Vaikimisi, kõik kasutajad, kontaktide, rühmade ja Windows 10 arvuti kontod on sünkroonitud. Saate kaasata või välja jätta vastavalt domeenid, organisatsiooniüksused või atribuudid objektid. 
    
- [Parooli räsi syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sünkroonib parooli räsi asutusesisese Active Directory Azure AD. See võimaldab salasõnade haldus ühes kohas, kuid kasutada sama parooli nii asutusesisese ja pilve keskkondades. Sest Active Directory on usaldusväärne allikas, saate oma parooli poliitika. 
    
- [Iseteeninduse parooli lähtestada (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) võimaldab kasutajatel oma paroolide lähtestamiseks pilves samas eelnevatega kohapeal paroolipoliitika. 
    
- [Seadme tagasikirjutusega](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) võimaldab registreeritud seadmed tuleb kirjutada tagasi asutusesisese Active Directory, nii et neid saab kasutada juurdepääsu Azure AD. 
    
- [Juhusliku oovin](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) lubatakse vaikimisi, et vältida liiga palju samaaegseid objekti kustutamist (üle 500 objekti sünkroonimise kohta). Saate muuta seda sätet vastavalt organisatsiooni vajadustele. 
    
- [Automaatne versioonitäiendus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on vaikimisi kiire käitiste ja tagada teie versioon Azure AD ühenduse on alati ajakohane. 
    

