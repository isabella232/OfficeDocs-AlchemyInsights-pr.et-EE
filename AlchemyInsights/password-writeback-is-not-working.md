---
title: Parooli tagasikirjutusega ei tööta
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243363"
---
# <a name="password-writeback-is-not-working"></a>Parooli tagasikirjutusega ei tööta

**Mul on probleeme parooli tagasikirjutusega konfigureerimisega**

- Salasõna tagasikirjutusega on esmaklassiline funktsioon.
- Veenduge, et mõistate litsentsimise nõudeid.
  - Teie ettevõttes peab olema vähemalt ühe litsentsiga määratud litsents.
  - **Ainult pilveteenuse kasutajad** – kõik Office 365 (O365) makstud SKU või Azure AD ' i põhifunktsioonid
  - **Pilv ja/või kohapealsed kasutajad** – Azure AD Premium P1 või P2, Enterprise Mobility + Security (EMS) või Secure produktiivne Enterprise (SPE)
    - Lisateavet litsentsimise nõuete kohta leiate teemast [AZURE ad iseteeninduse parooli lähtestamise litsentsimise nõuded](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Teil on vähemalt ühe administraatori konto ning ühe vastava litsentsiga kasutajakonto.
- Peate ühendama Azure AD Connecti esmase domeenikontrolleri Emulaatoriga tagasikirjutusega töötamiseks. Saate konfigureerida Azure AD Connecti kasutama esmast domeenikontrollerit, paremklõpsates Active Directory sünkroonimise konnektori **atribuute** ja valides seejärel käsu **Konfigureeri kausta partitsioonid**. Sealt otsige üles jaotis **domeenikontrolleri ühenduste sätted** ja märkige ruut nimega **ainult eelistatud domeenikontrollerid**.
  > [!NOTE]
  > Kui eelistatud DC pole PDC-emulaator, jääb Azure AD Connecti jaoks endiselt välja PDC parooli tagasikirjutusega.
- Parooli lähtestamine on teie rentniku jaoks konfigureeritud ja lubatud. Lisateavet leiate teemast [kasutajatele Azure ' i reklaami paroolide lähtestamise lubamine](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Veenduge, et administraatorikonto, mida kasutatakse parooli tagasikirjutusega lubamiseks, on pilveteenuse administraatorikonto (loodud Azure AD-s, mis pole kohapealne AD)
- Teil on ühe või mitme metsaga AD kohapealne juurutus, kus töötab Windows Server 2008 R2, Windows Server 2012 või Windows Server 2012 R2 uusimate hoolduspaketid installitud
- Teil on installitud Azure AD Connecti tööriist ja olete valmis oma reklaami keskkonna sünkroonimiseks pilve. Enne parooli tagasikirjutusega katsetamist veenduge, et täidate Azure AD Connecti kaudu nii AD kui ka Azure AD-st täieliku importimise ja täieliku sünkroonimise.
- Lisateavet leiate artiklist [AZURE ad Connecti täielik sünkroonimine ja täielik importimine](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Mul on probleem parooliga tagasikirjutusega ühenduvusega**

1. [AZURE ad Connecti](https://www.microsoft.com/download/details.aspx?id=47594) uusima versiooni allalaadimine ja lubamine
2. Tulemüüri konfigureerimine: Azure AD Connecti tööriist (1.1.443 ja ülal) vajab **VÄLJAMINEVA https** -i juurdepääsu:
    - passwordreset.microsoftonline.com
    - ServiceBus. Windows. Networks
3. Lubada, et idle ühendused püsivad vähemalt 2-3 minutit.

**Mul on endiselt probleeme parooliga tagasikirjutusega**

- Kui teil on endiselt probleeme, proovige keelata ja uuesti lubada parooli tagasikirjutusega teenus Azure AD Connecti tööriistas
- Lisateavet leiate teemast [parooli tagasikirjutusega keelamine ja uuesti lubamine](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
