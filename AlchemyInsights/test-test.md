---
title: SharePoint Online ' i Termini salvest puuduvad terminid
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750447"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLockeri krüptimise lubamine Intune ' i abil

Intune Endpoint Protection Policy saab kasutada Windowsi seadmete Boitlocker konfigureerimiseks, nagu on kirjeldatud jaotises: Windows10 (ja uuemad) sätted, et kaitsta seadmeid Intune ' i abil

Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10, toetavad automaatset BitLockeri krüptimist, mis käivitatakse MDM-poliitikat rakendamata. See võib mõjutada poliitika rakendamist, kui vaikesätted pole konfigureeritud. Üksikasjalikumat teavet leiate teemast KKK.


KKK   k: millised Windowsis olevad väljaanded toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?
 V: Intune ' i lõpp-punkti kaitsepoliitika sätted rakendatakse BitLockeri CSP-i kaudu.BitLockeri CSP ei toeta kõiki väljaandeid ega Windowsi väljaandeid. 
      Praegu on Windowsi versioonid: Enterprise; Toetatakse haridust, mobiili, mobiilset ettevõtlust ja Professionalit (alates järgust 1809).




K. Kui seade on BitLocker-iga juba krüptitud, kasutades krüptimise meetodi ja šifri tugevuse (XTS-AES-128) sätteid, mis käivitab automaatselt draivi uuesti krüpteerimise uute sätetega.

Vastus. Ei. Uute šifri sätete rakendamiseks peab draiv esmalt dekrüptima.

Märkus seadmete registreerimisel autopiloot on automaatne krüptimine, mis ilmneb OOBE ajal ei käivitu kuni Intune poliitika hinnatakse, mis võimaldab poliitikal põhinevad sätted, mida kasutatakse OS-i vaikesätete asemel




K kui seade krüptitakse Intune ' i poliitika rakendamise tõttu, dekrüptitakse see poliitika eemaldamise korral?

A: krüptimise seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimist.




K: Miks Intune ' i nõuetele vastavuse poliitika näitab, et minu seadmel pole "BitLocker enabled", kuid see on?

V: "BitLockeri lubatud" säte Intune ' i nõuetele vastavuse poliitikas kasutab Windowsi seadme terviseohutuse kinnitust (DHA) klienti. See klient mõõdab ainult seadme olekut alglaadimise ajal. Nii et kui seadet pole uuesti käivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeeninduse teenusest BitLocker aktiivsena.