---
title: Terminid puuduvad SharePoint veebitermini poest
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106419"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlockeri krüptimise lubamine Intune'iga

Intune'i lõpp-punkti kaitse poliitikat saab kasutada Boitlockeri krüptimissätete konfigureerimiseks Windows seadmete jaoks, nagu on kirjeldatud artiklis : Windows10 (ja uuemad) sätted Seadmete kaitsmiseks Intune'i abil

Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10 toetavad automaatset bitlockeri krüptimist, mis käivitatakse ilma MDM-i poliitika rakendamiseta. See võib mõjutada poliitika kohaldamist, kui vaikesätted pole konfigureeritud. Üksikasjalikumat teavet leiate teemast KKK.


KKK K. Millised Windows toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?
A. Intune'i lõpp-punkti kaitsepoliitika sätted rakendatakse Bitlockeri CSP-ga.  Bitlockeri CSP-d ei toeta Windows väljaanded ega järgud. Praegu on Windows Väljaanded: Enterprise; Toetatakse haridust, mobiilsidet, mobiilsideettevõtet ja professionaalset ettevõtet (alates 1809. aastast).




Küsimus. Kui seade on bitlockeriga juba krüptitud, kasutades krüptimismeetodi ja šifri tugevuse (XTS-AES-128) OS-i vaikesätteid, käivitab erinevate sätetega poliitika automaatselt ketta uuesti krüptimise uute sätetega?

Vastus. Ei. Uute šifrisätete rakendamiseks tuleb ketas esmalt dekrüptida.

Märkus. Automaatpilootiga registreerunud seadmete puhul ei käivitu OOBE ajal toimuv automaatne krüptimine enne Intune'i poliitika hindamist, mis võimaldab kasutada poliitikapõhiseid sätteid os-i vaikesätete asemel.




K. Kui seade on Intune'i poliitika rakendamise tulemusena krüptitud, dekrüptitakse see selle poliitika eemaldamisel?

A. Krüptimisega seotud poliitika eemaldamine ei tähenda konfigureeritud draivide dekrüptimist.




Küsimus. Miks näitab intune'i vastavuspoliitika, et minu seadmel pole "Bitlocker Enabled", kuid see on?

V. Intune'i vastavuspoliitika säte "Bitlocker enabled" kasutab Windows seadme seisundi tõendamise (DHA) klientrakendust. See klientrakendus liiab seadme olekut ainult alglaadimise ajal. Seega, kui seadet pole pärast bitlockeri krüptimise lõpetamist taaskäivitatud, ei teata DHA klientteenus bitlockerist aktiivsena.