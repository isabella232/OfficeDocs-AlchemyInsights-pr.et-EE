---
title: Tingimusjuurdepääsu blokeerib mind ühilduv seade
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019144"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Tingimusjuurdepääsu blokeerib mind ühilduv seade

**Väga soovitatavad tööriistad**

- [Seadme registreerimise tõrkeotsija tööriist –](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) põhjalik tööriist, mis aitab teha tõrkeotsingut kõige levinumatele seadme registreerimisega seotud probleemidele.
- [Seadme registreerimise ühenduvuse skript](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – tööriist, mille abil tagatakse seadmele juurdepääs seadme registreerimise lõpp-punktidele süsteemikonto kaudu.
- [Azure AD-seadme puhastusskript](https://github.com/mzmaili/AzureADDeviceCleanup) – tööriist, mida kasutatakse aegunud seadmete otsimiseks ja haldamiseks teie keskkonnas.

Siin on mõned levinumad põhjused, miks tingimusjuurdepääs võib  nõuetele vastavas seadmes nurjuda või miks teie kasutajad võivad saada teavet selle kohta, et te ei saa siit teavet ettevõtte ressursi sisselogimistaotluse ajal.

1. **Seade pole MDM-iga nõutavas seadme olekus.**

Kontrollige, kas seade on registreeritud koos kinnitatud MDM-i pakkujaga (nt Intune) ja *märgitud nõuetele vastavaks.* Lisateavet Intune'i kohta leiate sellest [dokumendist.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Seadme nõuetele vastavuse ja Intune'i kohta leiate lisateavet teemast Nõuetele vastavuse poliitika kasutamine [Intune'iga hallatavate seadmete reeglite häälestamiseks.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Kui teil on Intune'iga seadme registreerimisega probleeme, leiate tõrkeotsingu üksikasjad jaotisest Seadme [registreerimise tõrkeotsing Microsoftis.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Täiendava Intune'i toe saamiseks looge tugiteenusetaotlus. Selleks külastage [lehte Intune'i spikker ja tugi](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Seade pole ühendatud ettevõttevõrguga:**

Ettevõtte ressurssidele juurdepääsuks peab seade olema ühendatud ettevõtte võrguga kas otseühenduse või virtuaalse privaatvõrgu (VPN) kaudu ning olema ühendatud ettevõttesisese või Azure Active Directory. Tööseadme organisatsioonivõrguga liitumiseks lugege teemat [Tööseadmega liitumine ettevõtte võrku.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Isikliku/BYOD-seadme registreerimiseks lugege teemat Isikliku [seadme registreerimine ettevõtte võrgus.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Selleks et kontrollida, kas seade on võrguga liitunud, [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) saate siin või tööseadmetes järgida registreeritud seadmete [juhiseid.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Probleemi ulatuseks organisatsiooni võrguühendusse järgige alltoodud juhiseid.

    1. Logige sisse Windows oma töö- või koolikontoga (nt alain@contoso.com).
    2. Ühendus oma ettevõtte võrku VPN-i või DirectAccessi kaudu.
    3. Kui olete ühenduse loonud, vajutage **seadme Windows klahvi + L.**
    4. Vabastage seade töö- või koolikonto abil ja proovige seejärel probleemsele rakendusele või teenusele uuesti juurde pääseda.

Kui kuvatakse tõrketeade Te ei saa siia **enam enam,** on probleem tõenäoliselt mujal.

3. **Opsüsteemi ei toetata.**

Veenduge, et kasutate operatsioonisüsteemi toetatud versiooni, sh järgmist.

- **Windows Klient:** Windows 7 või uuem

- **Windows Server:** Windows Server 2008 R2 või uuem

- **macOS**: macOS X või uuem

- **Android ja iOS:** Androidi ja iOS-i mobiilsideseadmete uusim versioon

4. **Veebibrauserit ei toetata.**

Allpool leiate toetatud brauserid. Chrome'i toe Windows 1703 või uuemate versioonide korral on Windows 10 kontolaiend. Edge 85+ korral peab kasutaja seadme nõuetele vastavuse teabe õigeks läbimiseks sisse logima. Lisateavet leiate [siit](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Lisateavet leiate teemast **Sõnumi- ja** tõrkeotsingu juhised leiate [siit.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
