---
title: Microsoft Intune ' i Androidi seadmete registreerimisega seotud probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689950"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune ' i Androidi seadmete registreerimisega seotud probleemide tõrkeotsing

Probleemi lahendamiseks vaadake allpool loetletud ressursid üle.
  
Levinud probleemid ja lahendamise juhised.
  
 **Seadmes pole krüptitud tõrget ettevõtte portaalis.** Androidi uuemad versioonid, eriti alates v 7.0-st, vajavad käivituse pääsukoodi, et veenduda, kas teie seade on täielikult krüptitud. Levinumad lahendused on lubada käivitamise PIN-koodi või seadme täielikku krüptimist. Lisateabe saamiseks lugege [see dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) üle.
  
 **Seadmed ei suuda sisse logida Intune ' i teenusega või kuvada Intune ' i konsoolis "ebatervis".** Mõned Samsungi 4,4 ja 5,5 seadmed ei pruugi teenust sisse möllida. Sellele probleemile on kolm võimalikku lahendust.
  
1. Avage käsitsi Intune ' i ettevõtte portaali rakendus, mis käivitab automaatselt seadme sünkroonimise.

2. Värskendage seadet Androidi 6,0 või uuema versiooniga.

3. Keelake Samsung Smart Manager Intune ettevõtte portaali haldamisel. Vaadake üle [selle dokumendi](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) Lisateavet nende probleemide ja resolutsioonide kohta.

 **Kasutaja litsentsi tüüp on vigane** või **kasutaja nimi pole tuvastanud tõrge:** kasutajale tuleb määrata Intune või EMS-i litsents. Vaadake need dokumendid üle, et määrata litsents: Office halduskeskus või Azure ' i portaal.
  
Probleemi lahendamiseks täiendavad ressursid.
  
1. Saate kasutada [Intune tõrkeotsingu portaali](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) levinud liitumise tõrgete diagnoosimiseks ja lahendamiseks. Lisateabe saamiseks vaadake [seda dokumenti](https://docs.microsoft.com/intune/help-desk-operators) üle.

2. Vaadake üle [see dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) levinud tõrgete loend, mis takistavad iga kasutaja registreerimist ja eraldusvõimet.

3. [Siit saate teada, kuidas Microsoft Intune ' is Androidi seadmeid registreerida](https://docs.microsoft.com/intune/android-enroll).
