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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768813"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLockeri krüptimise lubamine Intune ' i abil

 Intune Endpoint Protection Policy saab kasutada BitLockeri krüptimise sätete konfigureerimiseks Windowsi seadmetes. Lisateavet leiate artiklist [Windows 10 (ja hilisemad) sätted, et kaitsta seadmeid Intune ' i abil](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10, toetavad automaatset BitLockeri krüptimist, mis käivitatakse MDM-poliitikat rakendamata. See võib mõjutada poliitika rakendamist, kui vaikesätted pole konfigureeritud. Üksikasjalikumat teavet leiate järgmisest KKK-s.
 
Lisateavet BitLockeri probleemide tõrkeotsingu kohta leiate teemast [BitLockeri poliitikate tõrkeotsing Microsoft Intune ' is](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**KKK**

K: millised Windows ' i versioonid toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?<br>
V: Intune ' i lõpp-punkti kaitsepoliitika sätted rakendatakse [BITLOCKERI CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)-i kaudu. BitLockeri CSP ei toeta kõiki Windowsi väljaandeid ega väljaandeid. <br><br>

K: Kuidas saab BitLockeri lubada seadmetes, nõudmata lõppkasutaja suhtlust?<br>
V: seni, kuni vajalikud eeltingimused on täidetud, on võimalik, et BitLocker "Silent Encryption" saab Intune ' i kaudu lubada. Lugege seadme nõuete ja näitepoliitika sätete üksikasju, et lubada vaikiva krüptimise lubamine järgmises dokumendis. [lubage BitLockeri krüptimine vaikselt](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

K. Kui seade on BitLocker-iga juba krüptitud, kasutades krüptimise meetodi ja šifri tugevuse (XTS-AES-128) jaoks mõeldud OS-i vaikesätteid, siis käivitab uue sättega automaatselt draivi uuesti krüptimine.<br>
Vastus. Ei. Uue šifri sätete rakendamiseks peab draiv esmalt dekrüptima.<br><br>
**Märkus:** Kui seadmeid registreeritakse autopiloodiga, siis OOBE ajal ilmnev automaatne krüptimine ei käivitu enne, kui poliitika on hinnanud, mis võimaldab OPERATSIOONISÜSTEEMI vaikesätete asemel kasutada poliitikal põhinevaid sätteid.
 
K. Kui seade krüptitakse Intune ' i poliitika rakendamise tõttu, dekrüptitakse see poliitika eemaldamise korral?<br>
V: krüptimisega seotud poliitika eemaldamine ei põhjusta konfigureeritud draivide dekrüptimist.
 
K: Miks Intune ' i nõuetele vastavuse poliitika näitab, et minu seadmel pole BitLockerit lubatud, isegi kui see on nii?<br>
V: Intune ' i nõuetele vastavuse poliitikas säte "BitLocker enabled" kasutab Windowsi seadme terviseohutuse kinnitust (DHA) klienti. See klient mõõdab ainult seadme olekut alglaadimise ajal. Nii et kui seadet pole uuesti käivitatud, kuna BitLockeri krüptimine on lõpule viidud, ei teata DHA klienditeeninduse teenusest BitLocker aktiivsena.
 
 