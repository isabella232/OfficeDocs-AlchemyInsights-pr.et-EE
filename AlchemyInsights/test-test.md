---
title: SharePoint Online ' i Terminikauplus puuduvad terminid
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053509"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLockeri krüptimise lubamine Intune ' iga

Intune lõpp-punkti kaitse poliitika saab konfigureerida Boitlocker krüpteerimise sätted Windowsi seadmete nagu kirjeldatud: Windows10 (ja uuem) sätteid, et kaitsta seadmeid, kasutades Intune

Peaksite teadma, et paljud uuemad seadmed, mis töötavad Windows 10 toetavad automaatset BitLockeri krüptimist, mis käivitatakse ilma MDM-poliitika rakendamist. See võib mõjutada poliitika rakendamist, kui vaikimisi sätted on konfigureeritud. Üksikasjalikumat infot leiate KKK-st.


KKK  Q: millised Windowsi tugiteenuste seadme krüptimine lõpp-punkti kaitse poliitika abil?
 A. Intune lõpp-punkti kaitse poliitika sätted rakendatakse BitLockeri CSP abil.Kõik väljaanded ega järkude Windows ei toeta BitLockeri CSP. 
      Sel ajal Windowsi väljaanded: Enterprise; Haridus, mobiil, mobiilne ettevõtlus ja professionaalne (alates järk 1809) toetatakse.




Q: kui seade on juba krüpteeritud BitLocker kasutades OPERATSIOONISÜSTEEMI vaikesätteid krüptimismeetod ja šifri tugevus (XTS-AES-128) kohaldab poliitika erinevate sätetega automaatselt käivitab uuesti krüpteerimine draivi uute sätetega?

A: ei. Uue šifri sätete rakendamiseks tuleb draiv esmalt dekrüptida.

Märkus seadmete registreerunud autopiloot automaatne krüptimine, mis ilmneb OOBE ajal ei käivitata enne Intune poliitika hinnatakse, mis võimaldab poliitika põhinev sätted kasutatakse asemel OS vaikesätted




Q kui seade on krüptitud tõttu rakenduse Intune poliitika on dekrüptida, kui see poliitika eemaldatakse?

A. krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimine.




Q: Miks Intune vastavuse poliitika näitab, et minu seade ei ole "BitLocker lubatud", kuid see on?

A: "BitLockeri lubatud" säte Intune vastavuse poliitika kasutab Windows seadme tervise kinnitus (DHA) klient. See klient mõõdab ainult seadme oleku boot ajal. Nii et kui seadet pole taaskäivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeenus BitLockeri aktiivsest seadmest.