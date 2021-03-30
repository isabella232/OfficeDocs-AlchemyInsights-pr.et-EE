---
title: Öövalguse kuvamissätte spikker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404399"
---
# <a name="help-with-the-night-light-display-setting"></a>Öövalguse kuvamissätte spikker

Ööaja kuvamissätete kohta leiate lisateavet teemast Windows 10 ööaja [kuvamisaja konfigureerimine.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Kui öövalguse suvandid on jaotises Sätted tuhm, kontrollige oma kuvadraiverit. 

1. Klõpsake tegumiribal otsinguvälja ja tippige **seadmehaldur** ja seejärel **valige** otsingutulemitest Seadmehaldur.
1. Laiendage **valikut Kuvaadapterid.** 

Kahjuks pole öövalguse funktsioon saadaval, kui teie seade kasutab DisplayLinki draiverit või põhikuvadraiverit.

Öövalguse funktsioon kasutab hiljutist graafikatehnoloogiat, nii et võib juhtuda, et peate kuvadraiverit värskendama.  

- Värskenduste otsimiseks valige Start  >  **Settings**  >  **Update & Security** Windows  >  **Update** Check  >  **for Updates**....  

OR

- Uusimate kuvadraiverite käsitsi allalaadimiseks ja installimiseks külastage riistvara tootja tugiteenuste veebisaiti.

## <a name="reset-night-light-in-the-registry"></a>Öine tule lähtestamine registris

Kui kuvadraiveri värskendamine ei toiminud, peate võib-olla lähtestama registris öövalguse.  

**Ettevaatust.** See tõrkeotsingut juhis on soovitatav ainult kogenud kasutajatele. Kui muudate registrit valesti, võivad ilmneda tõsised probleemid. Lisakaitse tagamiseks varundage register enne selle muutmist, et saate selle probleemide korral taastada.

1. Tippige otsinguväljale tekst **regedit** ja seejärel **valige** otsingutulemitest Registriredaktor.

1. Avage järgmine registrivõti. 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Eksportige ja kustutage järgmine alamvõti:$$windows.data.bluelightreduction.bluelightreductionstate

1. Eksportige ja kustutage järgmine alamvõti:$$windows.data.bluelightreduction.settings

1. Taaskäivitage Windows ja kontrollige, kas öövalgustuse suvandid on saadaval.


