---
title: Ma saan blokeeritud domeeniga liitunud seadmega tingimisi juurdepääsu tõttu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035723"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Ma saan blokeeritud domeeniga liitunud seadmega tingimisi juurdepääsu tõttu

**Väga Soovitatavad tööriistad**

[Seadme registreerimise tõrkeotsija tööriist](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – tööriist, mis aitab tõrkeotsingul kõige levinumaid seadme registreerimise probleeme.

[Seadme registreerimise ühenduvuse skriptimine](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – skript, mis aitab tagada, et seade pääseb juurde seadme registreerimise lõpp-punktidele süsteemi konto all.

[AZURE ad Device cleanup script](https://github.com/mzmaili/AzureADDeviceCleanup) – skript, mis võimaldab teil otsida ja hallata aegunud seadmeid teie keskkonnas.

Siin on mõned levinumad põhjused, miks tingimusjuurdepääsu võib nurjuda, kui seade on domeeniga liitunud (hübriid-Azure AD).

1. **Seadmes pole AZURE ad PRT** -d, peate veenduma, et seadmel on Azure AD esmase värskendamise luba (PRT). Lisateavet PRT kohta leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Kui soovite kontrollida, kas teil on Azure AD PRT, saate käivitada `dsregcmd/status` seadmes käsu ja kontrollida, kas "AzureAdPrt" võrdub "Jah".

Kui "AzureAdPrt" on "ei", siis kontrollige järgmist.

- **Kas teil on väline keskkond AD FS-iga ja see pole kasutajate koduvõrgust** juurdepääsetav: sel juhul veenduge, et teie "usernamemixed" lõpp-punktid on Suhtevõrgu kaudu juurdepääsetavad. Kui teie AD FS on VPN-i taga, veenduge, et kasutajad ühenduvad VPN-iga ja logige seadmesse uuesti sisse. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Kas seadme TPM on vigane ja seetõttu ei saa seadet autentida**: märkige ruut "TPM. msc", et näha, kas TPM-i olek on "valmis". Kui ei, siis käivitage `dsregcmd/leave` ja laske seadmel uuesti AZURE ad-ga liituda. Seejärel proovi uuesti. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Kasutate kolmanda osapoole identiteedi pakkujat, mis ei toeta WS-Trust protokolli**. Nagu on kirjeldatud meie dokumentides, ei saa hübriid-Azure AD-liitunud seadmed sel juhul töötada. Palun tööta oma identiteedi pakkujaga toe saamiseks.

2. **Kasutajad kasutavad Chrome ' i brauserit, ilma et Windows 10 kontod** või **Office ' i laiendus Chrome ei kasuta automaatselt PRT-ga liitunud või hübriid-AAD-ga ühendatud seadmetes PRT**. see viib tõrkele mis tahes seadmel põhinevate tingimusjuurdepääsu poliitikate korral, kus kuvatakse tõrketeade "registreerimata seade". Chrome ' i brauseri õigeks kasutamiseks peate installima "Windows 10 Accounts" või "Office ' i laienduse kasutajate Chrome ' i brauseris" SCCM või Intune ' i kaudu. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Kui laiendust ei saa eemalt tõugata, Teavitage kasutajaid käsitsi installimisest mõnele ülaltoodud laiendist, et pääseda juurde rakendustele, mis jäävad Device-põhise tingimusjuurdepääsu juurde. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Seade oli õigesti hübriid AZURE ad liitunud, kuid see on tahtmatult kustutatud või keelatud, kas AZURE ad Connecti või Azure ' i portaalis muudatuste sünkroonimise tõttu**: kui see on nii, siis seadme objekti ei tuvastata enam täielikult ühendatud seadmena, kuigi "AzureAdJoined" ja "PRT" olek kuvatakse seadmes kehtivana.

Selle probleemi lahendamiseks käivitage `dsregcmd/leave` mõjutatud seadmetes ja lubage uuesti AZURE ad. Lisateavet leiate sellest [dokumendist](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Kui teie seadmed on opsüsteemis Windows 10, 1809 Update, VPN-i/pilve puhverserveriga ja vaadake probleeme "AzureAdPrt" olekuga või mis tahes rakenduse SSO probleemiga (Outlook ei Ühenda postkastiga, isegi kui teil oli PRT), veenduge, et teil on see paik [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) või aprilli koondvärskenduses [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , et vältida PRT rikete tegemist.

















