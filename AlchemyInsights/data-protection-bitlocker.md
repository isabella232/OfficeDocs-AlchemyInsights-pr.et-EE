---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118570"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Bitlockeri krüptimise lubamine Intune'i abil

Intune'i lõpp-punkti kaitse poliitikat saab kasutada bitlockeri krüptimissätete konfigureerimiseks Windows seadmete jaoks. Lisateavet leiate teemast Windows 10 (ja uuemad) sätted seadmete [kaitsmiseks Intune'i abil.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Lisaks lõpp-punkti kaitse poliitikale on olemas ka krüptimisaruanne, mis annab üksikasjalikuma ülevaate seadmete krüptimisolekust. Sellele aruandele pääseb juurde MEM-i portaali jaotises Seadmed **> Monitor** ja seejärel valige jaotises **Konfiguratsioon** suvand [Krüptimisaruanne](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Kui leiate, et Bitlockeri ei saa ootuspäraselt lubada või et Bitlockeri lubamiseks kasutatav profiil on tõrke olekus, vaadake üle krüptimisaruanne, et paremini mõista, miks käitumine toimub.

Aruande tõlgendamise (sh erinevate krüptimisolekuväärtuste) kohta leiate lisateavet teemast Seadme [krüptimise jälgimine Intune'iga.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Peaksite teadma, et paljud uuemad seadmed, kus töötab Windows 10, toetavad automaatset Bitlockeri krüptimist, mis käivitatakse ilma MDM-i poliitika rakendamiseta. See võib mõjutada poliitika kohaldamist, kui vaikesätted pole konfigureeritud. Üksikasjalikumat teavet leiate järgmisest KKK-st.

Bitlockeri probleemide tõrkeotsingu kohta leiate teavet teemast [BitLockeri poliitikate tõrkeotsing Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**KKK**

Küsimus. Millised Windows toetavad seadme krüptimist lõpp-punkti kaitse poliitika abil?<br>
A. Intune'i lõpp-punkti kaitsepoliitika sätted rakendatakse [Bitlockeri CSP abil.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Bitlockeri CSP-d ei toeta Windows väljaanded ega järgud. <br><br>

Küsimus. Kuidas saab Bitlockeri lubada seadmetes ilma lõppkasutaja suhtlust nõudmata?<br>
A. Seni, kuni vajalikud eeltingimused on täidetud, on võimalik Bitlockeri "Vaikne krüptimine" intune'i kaudu lubada. Vaadake seadme nõuete ja näidispoliitika sätete üksikasju vaikse krüptimise lubamiseks järgmises doc's: Silently Enable Bitlocker Encryption (Luba [Bitlockeri krüptimine).](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

K. Kui seade on bitlockeriga juba krüptitud, kasutades krüptimismeetodi ja šifri tugevuse os-i vaikesätteid (XTS-AES-128), käivitab erinevate sätetega poliitika automaatselt ketta uuesti krüptimise uute sätetega?<br>
Vastus. Ei. Uute šifrisätete rakendamiseks tuleb ketas esmalt dekrüptida.<br><br>
**Märkus.** Automaatpilootiga registreeritud seadmete puhul ei käivitu OOBE ajal toimuv automaatne krüptimine enne Intune'i poliitika hindamist, mis võimaldab poliitikapõhiseid sätteid kasutada opsüsteemi vaikesätete asemel.
 
K. Kui seade on Intune'i poliitika rakendamise tulemusena krüptitud, kas see dekrüptitakse selle poliitika eemaldamisel?<br>
A. Krüptimisega seotud poliitika eemaldamine ei tähenda konfigureeritud draivide dekrüptimist.
 
Küsimus. Miks näitab Intune'i vastavuspoliitika, et minu seadmes pole BitLocker lubatud, kuigi see on lubatud?<br>
V. Intune'i vastavuspoliitika säte "Bitlocker enabled" kasutab Windows seadme seisundi tõendamise (DHA) klientrakendust. See klientrakendus liiab seadme olekut ainult alglaadimise ajal. Seega, kui seadet pole pärast Bitlockeri krüptimise lõpuleviimist taaskäivitatud, ei teata DHA klientteenus Bitlockerist aktiivsena.
 
 