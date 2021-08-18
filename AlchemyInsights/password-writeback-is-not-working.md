---
title: Parooli tagasikirjutus ei tööta
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324919"
---
# <a name="password-writeback-is-not-working"></a>Parooli tagasikirjutus ei tööta

**Mul on probleeme parooli tagasikirjutuse konfigureerimisega**

- Parooli tagasikirjutus on premium-funktsioon.
- Veenduge, et mõistate litsentsimisnõudeid.
  - Teie ettevõttes peab olema määratud vähemalt üks litsents
  - **Ainult pilveteenuse kasutajad** – Office 365 (O365) tasuline SKU või Azure AD Basic
  - **Pilveteenuse ja/või kohapealne** kasutaja – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure Productive Enterprise (SPE)
    - Lisateavet litsentsimisnõuete kohta leiate teemast [Azure AD iseteeninduse parooli lähtestamise litsentsimisnõuded](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Teil on vähemalt üks administraatorikonto ja üks testkasutaja konto, kellel on üks sobiv litsents.
- Parooli tagasisaadmiseks peate Ühendus azure AD-d ühendama esmase domeenikontrolleri emulaatoriga. Azure AD Ühendus saab konfigureerida kasutama primaardomeenikontrollerit,  paremklõpsades Active Directory sünkroonimiskonnektori atribuute ja seejärel valides **kataloogisektsioonide konfigureerimise.** Sealt otsige domeenikontrolleri ühenduse **sätete** jaotist ja märkige ruut nimega kasuta ainult **eelistatud domeenikontrolleriid.**
    **Märkus.** Kui eelistatud DC pole PDC-emulaator, siis Azure AD Ühendus endiselt PDC-ga ühendust, et parool tagasi kirjutada.
- Parooli lähtestamine on teie rentnikus konfigureeritud ja lubatud. Lisateavet leiate teemast Kasutajate [Azure AD paroolide lähtestamise lubamine.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Veenduge, et parooli tagasikirjutuse lubamiseks kasutatav administraatorikonto on pilveadministraatori konto (loodud Azure AD-s, mitte kohapealne AD)
- Teil on üks või mitme metsaga AD kohapealne juurutus, kus töötab Windows Server 2008 R2, Windows Server 2012 või Windows Server 2012 R2 koos installitud uusimate hoolduspakettidega
- Teil on installitud Azure AD Ühendus tööriist ja olete oma AD-keskkonna pilveteenusega sünkroonimiseks ette valmistanud. Enne parooli tagasikirjutuse testimist veenduge, et enne Azure AD-st ja Azure AD-st täielikku importimist ja täielikku sünkroonimist Ühendus.
- Lisateavet leiate teemast Täielik sünkroonimine ja [täielik importimine Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations) Ühendus

**Mul on probleem parooli tagasikirjutuse ühenduvusega**

1. Laadige alla ja lubage [Azure AD Ühendus](https://www.microsoft.com/download/details.aspx?id=47594)
2. Tulemüüri konfiguratsioon. Azure AD Ühendus (1.1.443 ja eespool) peab olema väljamineva **HTTPS-i** juurdepääs:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Luba tühikäiguühendustel püsida vähemalt 2–3 minutit

**Mul on endiselt probleeme parooli tagasikirjutusega**

- Kui teil on endiselt probleeme, proovige Azure AD-tööriistas parooli tagasikirjutusteenus keelata ja Ühendus lubada
- Lisateavet leiate teemast Parooli [tagasikirjutuse keelamine ja uuesti lubamine](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
