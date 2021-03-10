---
title: Parooli ennistamise probleem
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
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694380"
---
# <a name="problems-resetting-password"></a>Parooli ennistamise probleemid

Järgnevalt on toodud mõned probleemid, mis võivad parooli ennistamisel ja võimalike lahenduste leidmisel tekkida.

**Mul on probleem, mille parooli lähtestamine pole muudes kategooriates kaetud**

- Veenduge, et teil on õigus paroole lähtestada. Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks. Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.
- Veenduge, et mõistate litsentsimise nõudeid.
    - Teie ettevõttes peab olema vähemalt ühe litsentsiga määratud litsents.
        - Ainult pilveteenuse kasutajad – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid
        - Pilv ja/või kohapealsed kasutajad – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)
        - Lisateavet litsentsimise nõuete kohta leiate artiklist [litsentsimise nõuded AZURE ad iseteeninduskeskuse parooli lähtestamiseks](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Mul on probleeme parooli lähtestamise poliitika seadmisega**

- Hiljuti rakendatud poliitikad võivad võtta mitu minutit, et dubleerida kogu andmekeskuste ja lõpp-punkte. Kehaline kaugus andmekeskuse mõjutab ka seda, kui kiiresti muudatusi rakendatakse.
- Test lõppkasutajaga, mitte administraatoriga ja väikese kasutajate kogumiga piloot. Azure ' i portaalis konfigureeritud poliitikad rakenduvad ainult lõppkasutajatele, mitte administraatoritele. Microsoft jõustab iga Azure ' i administraatori rolli jaoks tugeva vaike-kahe värava parooli lähtestamise poliitika (nt globaalne administraator, kasutajatoe administraator, paroolide haldur jne).
    - Lugege lisateavet [administraatorite poliitikate](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)kohta.

**Soovin juurutada parooli lähtestamise, kuid ma ei soovi, et kasutajad ei saaks täiendavat turbeteavet registreerida**

Andmete eelasustamine kasutajate jaoks, et nad ei peaks seda tegema! -Administraatorina saate määrata oma kasutajatele telefoni ja meili atribuudid enne, kui käivitate oma organisatsioonile parooli lähtestamise. Seda saate teha API, PowerShelli või Azure AD Connecti abil. Lisateavet leiate siit:
- [Parooli lähtestamise juurutamine, mis ei nõua kasutajatelt registreerumist](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Milliseid andmeid parooli lähtestamine kasutab?](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nupp "parooli lähtestamine" on Hall**

Teil pole õigust selle kasutaja paroole lähtestada. Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks. Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.

**Parooli lähtestamise tera ei kuvata**

Teil pole õigust paroole lähtestada. Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks. Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.

**Ma ei näe kohapealset integratsiooni Blade parooli lähtestamisel**

- Kohapealne Integration Blade kuvatakse ainult hübriid-keskkonnas – see tähendab, et kasutate kohapealse kasutaja paroolide manipuleerimiseks parooli tagasikirjutusega.
- Te ei näe seda tera, kui:
    - Te ei kasuta parooli tagasikirjutusega
    - Parooli tagasikirjutusega installi/ühenduvusega on probleeme
    - Azure AD Connecti installi/ühenduvusega on probleeme
    - Lisateavet tagasikirjutusega probleemide lahendamise kohta leiate teemast [parooli tagasikirjutusega tõrkeotsing](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Kasutaja parooli lähtestamine**

1. Logige Azure ' i portaali sisse sobiva administraatorina.
1. Valige kasutajad ja rühmad Blade, valige **Kõik kasutajad**.
1. Valige loendist kasutaja.
1. Valitud kasutaja jaoks valige **Ülevaade** ja seejärel klõpsake menüüribal käsku **Lähtesta parool**.
1. Järgige ekraanil kuvatavaid juhiseid.
    - Lähtestatakse ainult Azure ' i portaali toe parooli tagasikirjutusega.

**Ma lähtestan kohapealse kasutaja parooli Office 365 administraatori või Office 365 mobiilirakenduse kaudu, kuid kasutaja ei saa ikka sisse logida**

Selles portaalis pole parooli tagasikirjutusega toetatud. Lähtestage kasutaja parool uuesti Azure ' i portaalis – portal.azure.com

