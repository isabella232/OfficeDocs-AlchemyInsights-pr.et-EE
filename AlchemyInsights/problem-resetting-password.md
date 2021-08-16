---
title: Probleem parooli lähtestamisel
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039962"
---
# <a name="problems-resetting-password"></a>Parooli lähtestamise probleemid

Järgnevalt on toodud mõned probleemid, mis võivad parooli lähtestamisel ja võimalikele lahendustele vastu aimata.

**Mul on probleem parooli lähtestamisega, mida ei hõlma muud kategooriad**

- Veenduge, et teil oleks õigus paroolid lähtestada. Kasutajaparoolid saavad lähtestada ainult üld-, parooli- ja kasutajaadministraatorid. Üldadministraatorid saavad lähtestada ka muid õigustega administraatori paroole.
- Veenduge, et mõistate litsentsimisnõudeid.
    - Teie ettevõttes peab olema määratud vähemalt üks litsents
        - Ainult pilveteenuse kasutajad – Office 365 (O365) tasuline SKU või Azure AD Basic
        - Pilveteenuse ja/või kohapealne kasutaja – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure Productive Enterprise (SPE)
        - Lisateavet litsentsimisnõuete kohta leiate artiklist [Azure AD iseteeninduse parooli lähtestamise litsentsimisnõuded.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Mul on probleeme minu määratud paroolilähtestuspoliitika testimisega**

- Hiljuti rakendatud poliitikate paljunemiseks kõigis andmekeskustes ja lõpp-punktides võib aega võtta mitu minutit. Füüsiline kaugus andmekeskusest mõjutab ka seda, kui kiiresti muudatusi rakendatakse.
- Testige lõppkasutajat, mitte administraatorit ja katseprojekti väikese kasutajakomplektiga. Azure'i portaalis ainult konfigureeritud poliitikad kehtivad lõppkasutajatele, mitte administraatoritele. Microsoft jõustab mis tahes Azure'i administraatorirolli jaoks tugeva kahe väravaga parooli lähtestamise poliitika (näide: üldadministraator, kasutajatoe administraator, parooliadministraator jne).
    - Lisateave [administraatorite poliitikate kohta.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Soovin juurutada parooli lähtestamise, kuid ma ei soovi, et kasutajad registreeriks täiendavat turbeteavet**

Kasutajate andmete eelasustamine, et nad ei peaks! - Administraatorina saate määrata oma kasutajatele telefoni- ja meiliasuvaid atribuute enne oma ettevõttesse parooli lähtestamist. Selleks saate kasutada API-d, PowerShelli või Azure AD-Ühendus. Lisateavet leiate siit.
- [Parooli lähtestamise juurutamine ilma kasutajaid registreerimata](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Milliseid andmeid parooli lähtestamine kasutab?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Parooli lähtestamise nupp on tuhm**

Teil pole õigust selle kasutaja paroole lähtestada. Kasutajaparoolid saavad lähtestada ainult üld-, parooli- ja kasutajaadministraatorid. Üldadministraatorid saavad lähtestada ka muid õigustega administraatori paroole.

**Ma ei näe paroolilähtestussaaba**

Teil pole õigust paroole lähtestada. Kasutajaparoolid saavad lähtestada ainult üld-, parooli- ja kasutajaadministraatorid. Üldadministraatorid saavad lähtestada ka muid õigustega administraatori paroole.

**Ma ei näe parooli lähtestamises kohapealst integreerimissaaga**

- Kohapealne integreerimisleht kuvatakse ainult hübriidkeskkondades, mis tähendab, et kasutate paroolide tagasikirjutust, et manipuleerida asutusesisese kasutaja paroole.
- Seda tera ei näe, kui:
    - Te ei kasuta parooli tagasikirjutust
    - Parooli tagasikirjutuse installimise/ühenduvusega on probleeme
    - Azure AD Ühendus
    - Lisateavet parooli tagasikirjutusega seotud probleemide tõrkeotsingu kohta leiate teemast Parooli [tagasikirjutuse tõrkeotsing](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ma ei tea, kuidas kasutaja parooli lähtestada**

1. Logige Azure'i portaali sisse sobiva administraatorina.
1. Avage nuga Kasutajad ja rühmad, valige **Kõik kasutajad**.
1. Valige loendist kasutaja.
1. Valige valitud kasutaja jaoks **Ülevaade** ja seejärel klõpsake käsuribal nuppu **Lähtesta parool.**
1. Järgige ekraanil kuvatavaid juhiseid.
    - Parooli tagasikirjutust toetavad ainult Azure'i portaali kaudu tehtud lähtestamised.

**Lähtestan asutusesisese kasutaja parooli Office 365 haldusrakendus või Office 365 mobiilirakendusest**

Selles portaalis ei toetata parooli tagasikirjutust. Lähtestage kasutaja parool uuesti Azure'i portaalis – portal.azure.com

