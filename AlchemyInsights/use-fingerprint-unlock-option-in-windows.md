---
title: Sõrmejälje lukust vabastamise suvandi kasutamine Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971899"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sõrmejälje lukust vabastamise suvandi kasutamine Windows 10

**Sõrmejälje Windows Hello lubamine**

Sõrmejälje Windows 10 avamiseks peate sõrmejälje häälestama, lisades Windows Hello (Windows õppivad tuvastama) vähemalt ühe sõrme. 

1. Avage **Sätted > kontod > sisselogimissuvandid** (või klõpsake [siin).](ms-settings:signinoptions?activationSource=GetHelp) Kuvatakse saadaolevad sisselogimissuvandid. Näide.

    ![Sisselogimissuvandid.](media/sign-in-options.png)

2. Klõpsake või puudutage **Windows Hello sõrmejälge** ja seejärel **nuppu Häälesta**. Klõpsake Windows Hello nuppu **Alustamine**. Sõrmejäljeandur aktiveeritakse ja teil palutakse sõrm andurile asetada.

   ![Sõrmejäljeandur.](media/fingerprint-sensor.png)

3. Järgige juhiseid, mis paluvad teil sõrme korduvalt skannida. Kui see on valmis, saate lisada muid sõrmi, mida soovite sisselogimiseks kasutada. Järgmine kord, kui logite Windows 10 sisse, saate selleks kasutada oma sõrmejälge.

**Windows Hello Sõrmejälg pole sisselogimissuvandina saadaval**

Kui Windows Hello sisselogimissuvandites ei kuvata suvandit Sõrmejälg, tähendab see, et Windows ei tea teie arvutile manustatud sõrmejäljelugejat/skannerit või et süsteemipoliitika takistab selle kasutamist (nt teie arvutit haldab teie töökoht). Tõrkeotsinguks tehke seda. 

1. Valige **tegumiribal** nupp Start ja otsige **seadmehaldurit.**

2. Klõpsake või puudutage **seadmehalduri avamiseks.**

3. Laiendage seadmehalduris valikut Biomeetrilised seadmed, klõpsates selle rööpnoolt.

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. Teie sõrmejäljeskanner peaks olema loetletud biomeetrilise seadmena (nt Synaptics WBDI skanner).

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. Kui teie sõrmejäljeskannerit ei kuvata ja skanner on arvutisse integreeritud, minge arvuti tootja veebisaidile. Otsige arvutimudeli tehnilise toe jaotisest Windows 10, mida saate installida.

6. Kui skanner on arvutist eraldi (usb-seadme kaudu manustatud), minge skanneri tootja veebisaidile, et leida ja installida Windows 10 seadmedraiveri tarkvara teie skannerimudeli jaoks.
