---
title: Microsoft Intune'is Androidi seadmete registreerimisega seotud probleemide tõrkeotsing
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830938"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune'is Androidi seadmete registreerimisega seotud probleemide tõrkeotsing

Vaadake allpool loetletud ressursid üle, et probleem kohe lahendada.
  
Mõned levinumad probleemid ja lahendused.
  
 **Seadmes pole krüptitud tõrge ettevõtteportaalis.** Androidi uuemad versioonid, eriti alates versioonist v7.0, nõuavad käivituspääsukoodi, et veenduda, et teie seade on täielikult krüptitud. Levinud lahendused on lubada käivitusviga või krüptida seade täielikult. Lisateavet [leiate sellest](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) dokumendist.
  
 Seadmetel ei õnnestu Intune'i teenusega sisse logida või intune'i halduskonsoolis kuvatakse **"Ebatervislik".** Mõned Samsung 4.4 ja 5.5 seadmed ei pruugi teenusesse sisseregistreerida. Sellele probleemile on kolm võimalikku lahendust.
  
1. Avage intune'i ettevõtteportaali rakendus käsitsi, mis algatab automaatselt seadme sünkroonimise.

2. Värskendage seade versioonile Android 6.0 või uuem.

3. Keelake Samsung Smart Manager intune'i ettevõtteportaali haldamisel. Vaadake [see dokument läbi,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) et lisateavet nende probleemide ja lahenduste kohta.

 **Kasutajalitsentsi tüübi kehtetu** või tundmatu kasutajanime **tõrge:** kasutajale tuleb määrata Intune'i või EMS-i litsents. Vaadake need dokumendid üle, et määrata litsents office'i halduskeskuse või Azure'i portaali kaudu.
  
Täiendavad ressursid probleemi lahendamiseks.
  
1. [Intune'i tõrkeotsinguportaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) abil saate diagnoosida ja lahendada levinumaid registreerimistõrkeid. Lisateavet [leiate sellest](https://docs.microsoft.com/intune/help-desk-operators) dokumendist.

2. Vaadake [see dokument üle,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) et saada ülevaade levinumatest vigadest, mis takistavad igale dokumendile registreerimist ja lahendamist.

3. [Siit saate teada, kuidas registreeruda Microsoft Intune'is Androidi seadmeid.](https://docs.microsoft.com/intune/android-enroll)
