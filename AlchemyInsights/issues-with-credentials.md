---
title: Mandaadiga seotud probleemid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063627"
---
# <a name="issues-with-credentials"></a>Mandaadiga seotud probleemid

[Microsoft Identity Platform ja oauthi 2,0 Client mandaatide voog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) kirjeldab, kuidas programmeerida otse OAuthi 2,0 kliendi mandaatide andmise voogu.

**Kuidas hallata rakenduse parooli või serdi mandaati?**

Rakenduses Azure CLI saate kasutada [AZ AD Rakenduse mandaati](https://docs.microsoft.com/cli/azure/ad/app/credential) , et kustutada, loetleda või lähtestada rakenduse parooli või serdi mandaati.

**Kuidas saavad kasutajad oma paroolid lähtestada?**

Kasutajad peavad oma paroolide lähtestamiseks [registreerima end teenuse parooli lähtestamiseks](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) . Kui kasutaja on registreerunud, saavad nad oma parooli lähtestamiseks järgida selle artikli juhiseid: [töö või kooli parooli lähtestamine](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Kuidas saavad kasutajad oma paroole muuta?**

Kasutajad saavad selle artikli juhiseid järgides oma paroole muuta: [parooli muutmine](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Nad saavad ka [hallata rakenduse paroole kaheastmeline kinnitamiseks](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Kasutaja saab parooli muutmisel või lähtestamisel tõrketeate**

See link annab teavet levinud probleemide kohta, mis võivad tekkida siis, kui kasutaja proovib lähtestada parooli: [levinud probleemid ja nende lahendused](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mul on probleeme kasutaja parooli ennistamisega**

- Veenduge, et teil on õigus paroole lähtestada. *Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.* Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.

- Veenduge, et mõistate litsentsimise nõudeid.

  - Teie ettevõttes peab olema vähemalt ühe litsentsiga määratud litsents.
    - **Ainult pilveteenuse kasutajad** – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid
    - **Pilv ja/või kohapealsed kasutajad** – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)
    - Lisateavet litsentsimise nõuete kohta leiate teemast [AZURE ad iseteeninduskeskuse parooli lähtestamise litsentsimise nõuded](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Kasutaja parooli lähtestamiseks otsige üles Azure AD kasutaja. Seejärel klõpsake selle kasutaja ülevaates nuppu "Lähtesta parool".

**Nupp "parooli lähtestamine" on Hall**

Teil pole õigust **selle** kasutaja paroole lähtestada. *Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.* Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.

**Parooli lähtestamise tera ei kuvata**

Teil pole õigust paroole lähtestada. *Kasutaja paroole saab lähtestada ainult globaalsete, paroolide ja kasutajate administraatorite jaoks.* Globaalsed administraatorid saavad lähtestada ka muud privilegeeritud administraatori paroolid.

**Ma ei näe kohapealset integratsiooni Blade parooli lähtestamisel**

- Kohapealne Integration Blade kuvatakse ainult hübriid-keskkonnas – see tähendab, et kasutate kohapealse kasutaja paroolide manipuleerimiseks parooli tagasikirjutusega.

- Te ei näe seda tera, kui:

  - Te ei kasuta parooli tagasikirjutusega
  - Parooli tagasikirjutusega installi/ühenduvusega on probleeme
  - Azure AD Connecti installi/ühenduvusega on probleeme
  - Lisateavet tagasikirjutusega seotud probleemide tõrkeotsingu kohta leiate teemast [parooli tagasikirjutusega tõrkeotsing](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Kasutaja parooli lähtestamine**

1. Logige Azure ' i portaali sisse sobiva administraatorina.
2. Valige **kasutajad ja rühmad** Blade, valige **Kõik kasutajad**.
3. Valige loendist kasutaja.
4. Valitud kasutaja jaoks valige **Ülevaade** ja seejärel valige käsuriba käsk **Lähtesta parool**.
5. Valige nupp **Lähtesta parool** ja järgige ekraanil kuvatavaid juhiseid.
    - Lähtestatakse ainult **Azure ' i portaali** toe parooli tagasikirjutusega.

**Ma lähtestan kohapealse kasutaja parooli Office 365 administraatori või Office 365 mobiilirakenduse kaudu, kuid kasutaja ei saa ikka sisse logida**

Selles portaalis pole parooli tagasikirjutusega toetatud. Lähtestage kasutaja parool uuesti Azure ' i portaalis.
