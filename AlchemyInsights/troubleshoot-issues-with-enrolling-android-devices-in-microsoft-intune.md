---
title: Androidi seadmete registreerimisega seotud probleemide tõrkeotsing Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008074"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Androidi seadmete registreerimisega seotud probleemide tõrkeotsing Microsoft Intune

Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.
  
Mõned levinumad probleemid ja lahendused.
  
 **Seadmes pole krüptitud Company Portal.** Androidi uuemad versioonid, eriti alates versioonist v7.0, nõuavad käivituspääsukoodi, et veenduda, et teie seade on täielikult krüptitud. Levinud lahendused on lubada käivitusviga või krüptida seade täielikult. Lisateavet [leiate sellest](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dokumendist.
  
 Seadmetel ei õnnestu Intune'i teenusega sisse logida või intune'i halduskonsoolis kuvatakse **"Ebatervislik".** Mõned Samsung 4.4 ja 5.5 seadmed ei pruugi teenusesse sisseregistreerida. Sellele probleemile on kolm võimalikku lahendust.
  
1. Avage käsitsi Intune Company Portal rakendus, mis algatab automaatselt seadme sünkroonimise.

2. Värskendage seade versioonile Android 6.0 või uuem.

3. Keelake Samsung Smart Manageri Intune Company Portal. Vaadake [see dokument läbi,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) et lisateavet nende probleemide ja lahenduste kohta.

 **Kasutajalitsentsi tüübi kehtetu** või tundmatu kasutajanime **tõrge:** kasutajale tuleb määrata Intune'i või EMS-i litsents. Vaadake läbi need dokumendid, et määrata litsents Office või Azure'i portaali kaudu.
  
Täiendavad ressursid probleemi lahendamiseks.
  
1. [Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid. Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.

2. Vaadake [see dokument üle,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) et saada ülevaade levinumatest vigadest, mis takistavad igale dokumendile registreerimist ja lahendamist.

3. [Siit saate teada, kuidas registreerida Androidi Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
