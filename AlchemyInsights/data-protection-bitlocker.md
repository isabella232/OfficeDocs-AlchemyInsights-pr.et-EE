---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731235"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLockeri krüptimise lubamine Intune ' i abil

 Intune Endpoint Protection Policy saab kasutada BitLockeri krüptimise sätete konfigureerimiseks Windowsi seadmetes. Lisateavet leiate artiklist [Windows 10 (ja hilisemad) sätted, et kaitsta seadmeid Intune ' i abil](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10, toetavad automaatset BitLockeri krüptimist, mis käivitatakse MDM-poliitikat rakendamata. See võib mõjutada poliitika rakendamist, kui vaikesätted pole konfigureeritud. Üksikasjalikumat teavet leiate järgmisest KKK-s.
 
Lisateavet BitLockeri probleemide tõrkeotsingu kohta leiate teemast [BitLockeri poliitikate tõrkeotsing Microsoft Intune ' is](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**KKK**

 K: millised Windows ' i versioonid toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?<br>
 V: Intune ' i lõpp-punkti kaitsepoliitika sätted rakendatakse [BITLOCKERI CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-i kaudu. BitLockeri CSP ei toeta kõiki Windowsi väljaandeid ega väljaandeid. <br><br>
      Praegu toetatakse järgmisi Windowsi väljaandeid: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (järk 1809 ja uuem versioon).
 
K. Kui seade on BitLocker-iga juba krüptitud, kasutades krüptimise meetodi ja šifri tugevuse (XTS-AES-128) jaoks mõeldud OS-i vaikesätteid, siis käivitab uue sättega automaatselt draivi uuesti krüptimine.<br>
Vastus. Ei. Uue šifri sätete rakendamiseks peab draiv esmalt dekrüptima.<br><br>
**Märkus:** Kui seadmeid registreeritakse autopiloodiga, siis OOBE ajal ilmnev automaatne krüptimine ei käivitu enne, kui poliitika on hinnanud, mis võimaldab OPERATSIOONISÜSTEEMI vaikesätete asemel kasutada poliitikal põhinevaid sätteid.
 
K. Kui seade krüptitakse Intune ' i poliitika rakendamise tõttu, dekrüptitakse see poliitika eemaldamise korral?<br>
V: krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimist.
 
K: Miks Intune ' i nõuetele vastavuse poliitika näitab, et minu seadmel pole BitLockerit lubatud, isegi kui see on nii?<br>
V: Intune ' i nõuetele vastavuse poliitikas säte "BitLocker enabled" kasutab Windowsi seadme terviseohutuse kinnitust (DHA) klienti. See klient mõõdab ainult seadme olekut alglaadimise ajal. Nii et kui seadet pole uuesti käivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeeninduse teenusest BitLocker aktiivsena.
 
 