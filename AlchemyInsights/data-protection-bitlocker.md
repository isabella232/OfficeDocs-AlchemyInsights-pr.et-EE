---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908706"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLockeri krüptimise lubamine Intune ' iga

 Intune lõpp-punkti kaitse poliitika saab kasutada BitLockeri Krüptimissätete konfigureerimiseks Windowsi seadmetele. Lisateabe saamiseks vaadake [Windows 10 (ja uuemate versioonide) sätteid, et kaitsta seadmeid Intune ' i abil](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Peaksite teadma, et paljud uuemad seadmed, mis töötavad Windows 10 toetavad automaatset BitLockeri krüptimist, mis käivitatakse ilma MDM-poliitika rakenduseta. See võib mõjutada poliitika rakendamist, kui vaikesätted on konfigureeritud. Üksikasjalikumat Lisateavet leiate järgmistest KKK-st.
 
BitLockeri probleemide tõrkeotsingu kohta teabe saamiseks vaadake [Microsofti Intune BitLockeri poliitikate tõrkeotsing](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Kkk**

 Q: mis väljaanded Windowsi tugiteenuste seadme krüptimine lõpp-punkti kaitse poliitika abil?<br>
 A. Intune lõpp-punkti kaitse poliitika sätted rakendatakse [BitLockeri CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)abil. Kõik väljaanded või Windowsi järgud toetavad BitLockeri CSP. <br><br>
      Sel ajal toetatakse järgmisi Windowsi väljaandeid: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (järk 1809 ja uuem).
 
Q: kui seade on juba krüpteeritud BitLocker kasutades OPERATSIOONISÜSTEEMI vaikesätteid krüpteerimismeetod ja šifri tugevus (XTS-AES-128), rakendades poliitika erinevate sätetega automaatselt käivitab uuesti krüpteerimine draivi uute sätetega?<br>
A: ei. Uue šifri sätete rakendamiseks peab draiv esmalt dekrüpteeritud.<br><br>
**Märkus:** Autodele, mis on kaasatud autopiloot, automaatne krüptimine, mis ilmneb OOBE ajal ei käivitata enne Intune poliitika on hinnatud, mis võimaldab poliitikapõhise sätted kasutatakse asemel OS vaikesätted.
 
Q: kui seade on krüpteeritud tõttu rakenduse Intune poliitika, kas see dekrüpteeritakse, kui see poliitika eemaldatakse?<br>
A. krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimine.
 
Q: Miks Intune vastavuse poliitika näitab, et minu seadmel pole BitLockeri lubatud, kuigi see on?<br>
A: "BitLocker lubatud" säte Intune vastavuse poliitika kasutab Windows seadme tervise kinnitus (DHA) klient. See klient mõõdab ainult seadme oleku boot ajal. Nii et kui seadet pole taaskäivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeenindus BitLockeri aktiivsena.
 
 