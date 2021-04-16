---
title: Sõrmejälje lukust vabastamise suvandi kasutamine opsüsteemis Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796673"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sõrmejälje lukust vabastamise suvandi kasutamine opsüsteemis Windows 10

**Luba Windows Hello sõrmejälg**

Windows 10 avamiseks sõrmejälje abil peate häälestama Windows Hello sõrmejälje, lisades (lastes Windowsil ära tunda) vähemalt ühe sõrme. 

1. Avage **Sätted > Kontod > sisselogimissuvandid** (või klõpsake [siin).](ms-settings:signinoptions?activationSource=GetHelp) Kuvatakse saadaolevad sisselogimissuvandid. Näide.

    ![Sisselogimissuvandid.](media/sign-in-options.png)

2. Klõpsake või **puudutage valikut Windows Hello Fingerprint (Windows Hello sõrmejälg)** ja **seejärel nuppu Set up (Häälesta).** Klõpsake Windows Hello häälestusaknas **nuppu Alustamine.** Sõrmejäljeandur aktiveeritakse ja teil palutakse sõrm andurile asetada.

   ![Sõrmejäljeandur.](media/fingerprint-sensor.png)

3. Järgige juhiseid, mis paluvad teil sõrme korduvalt skannida. Kui see on valmis, saate lisada muid sõrmi, mida soovite sisselogimiseks kasutada. Järgmine kord, kui logite windows 10 sisse, saate selleks kasutada oma sõrmejälge.

**Windows Hello sõrmejälg pole sisselogimissuvandina saadaval**

Kui Windows Hello sõrmejälge ei kuvata sisselogimissuvandites suvandina, siis tähendab see, et Windows ei tea teie arvutile manustatud sõrmejäljelugejat/skannerit või et süsteemipoliitika takistab selle kasutamist (nt teie arvutit haldab teie töökoht). Tõrkeotsinguks tehke seda. 

1. Valige **tegumiribal** nupp Start ja otsige **seadmehaldurit.**

2. Klõpsake või puudutage **seadmehalduri avamiseks.**

3. Laiendage seadmehalduris valikut Biomeetrilised seadmed, klõpsates selle rööpnoolt.

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. Teie sõrmejäljeskanner peaks olema loetletud biomeetrilise seadmena (nt Synaptics WBDI skanner).

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. Kui teie sõrmejäljeskannerit ei kuvata ja skanner on arvutisse integreeritud, minge arvuti tootja veebisaidile. Otsige arvutimudeli tehnilise toe jaotisest windows 10 draiverit, mille saate installida.

6. Kui skanner on arvutist eraldi (usb-seadme kaudu manustatud), minge skanneri tootja veebisaidile, et leida ja installida Windows 10 seadmedraiveri tarkvara teie skannerimudeli jaoks.
