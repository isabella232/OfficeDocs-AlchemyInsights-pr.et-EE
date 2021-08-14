---
title: Identimisteabega seotud probleemid
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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986815"
---
# <a name="issues-with-credentials"></a>Identimisteabega seotud probleemid

[Microsofti identimisplatvorm ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) kliendi identimisteabe voog kirjeldab, kuidas otse OAuth 2.0 kliendi identimisteabe voo vastu programmeerida.

**Kuidas hallata rakenduse parooli või serdi identimisteavet?**

Azure'i CLI-s saate az [ad rakenduse](https://docs.microsoft.com/cli/azure/ad/app/credential) identimisteabe abil kustutada, loetleda või lähtestada rakenduse parooli või serdi identimisteavet.

**Kuidas kasutajad paroolid lähtestavad?**

Enne [paroolide lähtestamist peavad kasutajad](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) registreeruma iseteeninduse parooli lähtestamiseks. Kui kasutaja on registreerunud, saab ta parooli lähtestamiseks järgida selles artiklis toodud [juhiseid: Töö- või kooliparooli lähtestamine.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kuidas saavad kasutajad oma paroole muuta?**

Kasutajad saavad oma paroolide muutmiseks järgida selles artiklis toodud [juhiseid: Parooli muutmine.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Samuti saavad nad [rakenduseparoolide haldamine kaheastmelise kontrollimise jaoks.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mu kasutaja saab parooli muutmisel või lähtestamisel tõrketeate**

See link annab teavet levinumate probleemide kohta, mis võivad tekkida, kui kasutaja proovib parooli lähtestada: [levinumad probleemid ja nende lahendused](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Mul on probleem kasutaja parooli lähtestamisel**

- Veenduge, et teil oleks õigus paroolid lähtestada. *Kasutajaparoolid saavad lähtestada ainult üld-, parooli- ja kasutajaadministraatorid.* Üldadministraatorid saavad lähtestada ka muid õigustega administraatori paroole.

- Veenduge, et mõistate litsentsimisnõudeid.

  - Teie ettevõttes peab olema määratud vähemalt üks litsents.
    - **Ainult pilveteenuse kasutajad** – Office 365 (O365) tasuline SKU või Azure AD Basic
    - **Pilveteenuse ja/või kohapealne** kasutaja – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure Productive Enterprise (SPE)
    - Lisateavet litsentsimisnõuete kohta leiate teemast [Azure AD iseteeninduse parooli lähtestamise litsentsimisnõuded.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Kasutaja parooli lähtestamiseks otsige kasutaja üles Azure AD-s. Seejärel klõpsake selle kasutaja ülevaatesabas nuppu "Lähtesta parool".

**Parooli lähtestamise nupp on tuhm**

Teil pole õigust selle **kasutaja** paroole lähtestada. *Kasutajaparoolid saavad lähtestada ainult üld-, parooli- ja kasutajaadministraatorid.* Üldadministraatorid saavad lähtestada ka muid õigustega administraatori paroole.

**Ma ei näe paroolilähtestussaaba**

Teil pole õigust paroole lähtestada. *Kasutajaparoolid saavad lähtestada ainult üld-, parooli- ja kasutajaadministraatorid.* Üldadministraatorid saavad lähtestada ka muid õigustega administraatori paroole.

**Ma ei näe parooli lähtestamises kohapealst integreerimissaaga**

- Kohapealne integreerimisleht kuvatakse ainult hübriidkeskkondades, mis tähendab, et kasutate paroolide tagasikirjutust, et manipuleerida asutusesisese kasutaja paroole.

- Seda tera ei näe, kui:

  - Te ei kasuta parooli tagasikirjutust
  - Parooli tagasikirjutuse installimise/ühenduvusega on probleeme
  - Azure AD Ühendus
  - Lisateavet parooli tagasikirjutusega seotud probleemide tõrkeotsingu kohta leiate teemast [Parooli tagasikirjutuse tõrkeotsing](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ma ei tea, kuidas kasutaja parooli lähtestada**

1. Logige Azure'i portaali sisse sobiva administraatorina.
2. Avage **nuga Kasutajad ja rühmad,** valige **Kõik kasutajad**.
3. Valige loendist kasutaja.
4. Valige valitud kasutaja jaoks **Ülevaade** ja seejärel valige käsuribal Käsk **Lähtesta parool**.
5. Valige **nupp Lähtesta** parool ja järgige ekraanil kuvatavaid juhiseid.
    - Parooli tagasikirjutust toetavad ainult **Azure'i** portaali kaudu tehtud lähtestamised.

**Lähtestan asutusesisese kasutaja parooli Office 365 haldusrakendus või Office 365 mobiilirakendusest**

Selles portaalis ei toetata parooli tagasikirjutust. Lähtestage kasutaja parool Uuesti Azure'i portaalis.
