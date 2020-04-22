---
title: Microsofti Intune ' is olevate Android-seadmetega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759616"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsofti Intune ' is olevate Android-seadmetega seotud probleemide tõrkeotsing

Vaadake allpool loetletud ressursid probleemi lahendamiseks kohe.
  
Mõned levinud probleemid ja lahendus järgmiselt:
  
 **Seade pole krüptitud tõrge ettevõtteportaalis:** Androidi uuemad versioonid, eriti alates v 7.0, nõuavad käivituspääsukoodi veendumaks, et teie seade on täielikult krüpteeritud. Levinud lahendused on lubada käivituspin või täielikult krüptida seade. Vaadake [seda dokumenti](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lisateabe saamiseks.
  
 **Seadmed ei saa sisse möllimist Intune teenus või Kuva "Unhealthy" Intune konsoolis:** Mõned Samsung 4,4 ja 5,5 seadmed ei pruugi teenuse sisse mölanda. On 3 võimalikud lahendused sellele probleemile:
  
1. Avage käsitsi rakenduse Intune Company portaal, mis alustab automaatselt seadme sünkroonimist.

2. Värskendage seade Android 6,0 või uuem versioon.

3. Keelake Samsung Smart Manager Intune ettevõtte portaali haldamine. Vaadake [seda dokumenti](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) nende probleemide ja resolutsioonide kohta lisateabe saamiseks.

 **Kasutaja litsentsi tüüp kehtetu** või **kasutaja nimi tundmatu tõrge:** kasutaja peab olema määratud Intune või EMS litsents. Vaadake üle need dokumendid litsentsi määramiseks: Office ' i administreerimiskeskus või Azure ' i portaal.
  
Täiendavad ressursid probleemi lahendamiseks:
  
1. Levinud registreerimise tõrgete diagnoosimiseks ja lahendamiseks kasutage [tõrkeotsingu portaali Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) . Vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) rohkem üksikasju.

2. Vaadake [seda dokumenti](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) levinud tõrgete loendi, mis takistavad registreerimise ja resolutsioonide iga.

3. [Vaadake, kuidas registreeruda Android-seadmeid Microsoft Intune ' is](https://docs.microsoft.com/intune/android-enroll).
