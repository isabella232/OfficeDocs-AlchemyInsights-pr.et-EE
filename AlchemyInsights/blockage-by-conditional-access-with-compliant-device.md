---
title: Mul on keelatud juurdepääs nõuetele vastava seadmega
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035371"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Mul on keelatud juurdepääs nõuetele vastava seadmega

**Väga Soovitatavad tööriistad**

- [Seadme registreerimise tõrkeotsija tööriist](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – terviklik tööriist, mis aitab tõrkeotsingul kasutada levinumaid seadme registreerimise probleeme.
- [Seadme registreerimise ühenduvuse testimine](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – tööriist, mida kasutatakse selle tagamiseks, et seade pääseks juurde seadme registreerimise lõpp-punktidele süsteemi konto alusel.
- [AZURE ad Device cleanup script](https://github.com/mzmaili/AzureADDeviceCleanup) -tööriist, mida kasutatakse teie keskkonna aegunud seadmete otsimiseks ja haldamiseks.

Siin on mõned levinumad põhjused, miks tingimusjuurdepääsu võib olla lubamatu seadme jaoks või miks teie kasutajad ei **saa teile** sisse logida, kui teil on sisselogimise taotlusel asutuse ressurss.

1. **Seade pole nõutud seadmes, kus on MDM**.

Veenduge, et seadmesse on kaasatud kinnitatud MDM-pakkuja (nt Intune) ja *märgitud nõuetele vastavaks*. Lisateavet Intune ' i kohta leiate sellest [dokumendist](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Seadme nõuetele vastavuse ja Intune ' i paremaks mõistmiseks leiate teavet teemast [nõuetele vastavuse poliitikate häälestamine Intune ' iga hallatavatele seadmetele reeglite häälestamiseks](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Kui teil on probleeme Intune ' i seadmesse registreerimisega, leiate tõrkeotsingu üksikasjad veebisaidil [Microsoftis seadme liitumise tõrkeotsing](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Täiendavaks Intune ' i toe saamiseks looge tugiteenuste taotlus. Selleks avage leht Intune ' i [Spikker ja tugi](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Seade pole liitunud organisatsioonide võrguga**.

Organisatsiooni ressurssidele juurdepääsuks peab seade olema ühendatud organisatsiooni võrguga kas otsese ühenduse või virtuaalse privaatvõrgu (VPN-i) kaudu ning liitunud ka asutusesisese või Azure Active Directoryga. Tööseadmega liitumiseks organisatsiooni võrguga lugege artiklit [tööseadmega liitumine ettevõtte võrguga](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Isikliku/BYOD seadme registreerimiseks leiate teavet teemast [isikliku seadme registreerimine ettevõtte võrgus](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Kui soovite kontrollida, kas seade on võrguga liitunud, [saate siin registreeritud](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) seadmete juhiseid jälgida või [siin](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)töötada. Probleemi lahendamiseks organisatsiooniskeemi ühenduvuse jaoks järgige allolevaid juhiseid.

    1. Logige Windowsi sisse oma töökoha või kooli kontoga (nt alain@contoso.com).
    2. Loo ühendus oma ettevõtte võrguga VPN-i või DirectAccess kaudu.
    3. Kui ühendus on loodud, vajutage seadme lukustamiseks **Windowsi logoga klahvi + L** .
    4. Avage oma seadmes töö või kooli konto abil oma seade ja proovige probleemset rakendust või teenust uuesti juurde pääseda.

Kui näete, et **te ei saa siin** tõrketeate uuesti kohale jõuda, on probleem tõenäoliselt mujal.

3. **Operatsioonisüsteem pole toetatud**.

Veenduge, et käitate operatsioonisüsteemi toetatud versiooni, sealhulgas järgmist.

- **Windowsi klientrakendus**: Windows 7 või uuem versioon

- **Windows Server**: windows Server 2008 R2 või uuem versioon

- **MacOS**: MacOS X või uuem

- **Android ja iOS**: Androidi ja iOS-i operatsioonisüsteemide uusim versioon

4. **Veebibrauser pole toetatud**.

Palun Otsi allpool olevaid toetatud brausereid. Windows 1703 või uuemate versioonidega Chrome ' i toe jaoks on nõutav Windows 10 kontode laiend. Edge 85 + korral peab kasutaja olema sisse logitud seadme nõuetele vastavuse teabe õigeks edastamiseks. Lisateavet leiate [siit](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune ' i hallatav brauser, Safari
- **Android**: **Microsoft Edge**: hallatava brauseri Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

[Siit](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)leiate lisateavet selle kohta, **kas te ei saa seal** sõnumit ja tõrkeotsingujuhiseid.
