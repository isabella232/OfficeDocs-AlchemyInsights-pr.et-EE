---
title: Windows 10 sõrmejälgede avamise suvandi kasutamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795240"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Windows 10 sõrmejälgede avamise suvandi kasutamine

**Luba Windows Hello sõrmejälg**

Kui soovite Windows 10 oma sõrmejälgede abil vabastada, peate häälestama Windows Hello sõrmejälje, lisades (lastes Windows õppima ära tundma) vähemalt ühe sõrmega. 

1. Valige **sätted, > kontode > sisselogimise suvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)). Saadaolevad sisselogimise suvandid on loetletud. Näiteks.

    ![Sisselogimise suvandid.](media/sign-in-options.png)

2. Klõpsake või puudutage valikut **Windows Hello sõrmejälg**ja seejärel klõpsake nuppu **Häälesta**. Klõpsake Windowsi Hello häälestamise aknas nuppu **Alustamine**. Sõrmejäljelugeja aktiveerub ja teil palutakse sõrm sensori ette paigutada.

   ![Sõrmejälgede andur.](media/fingerprint-sensor.png)

3. Järgige juhiseid, mis paluvad teil sõrme korduvalt skannida. Kui see on valmis, on teil võimalus lisada muid sõrmi, mida soovite kasutada sisselogimiseks. Järgmine kord, kui logite sisse operatsioonisüsteemi Windows 10, on teil võimalus kasutada oma sõrmejälge.

**Windows Hello sõrmejälg pole sisselogimise suvandina saadaval**

Kui Windows Hello sõrmejälge ei kuvata **sisselogimise**suvandites, tähendab see seda, et Windows ei ole teadlik teie arvutiga ühendatud sõrmejäljelugeja/skannerist või et süsteemi poliitika takistab selle kasutamist (näiteks teie arvutit haldab teie töökoht). Tõrkeotsingu sooritamiseks tehke järgmist. 

1. Valige tegumiribal nupp **Start** ja otsige üles **Seadmehaldur**.

2. **Seadmehalduri**avamiseks klõpsake või koputage seda.

3. Seadmehalduris laiendage biomeetriliste seadmete klõpsamisel selle Chevron.

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. Teie sõrmejälgede skanner tuleks loetleda biomeetriliste seadmetena (nt Synaptics WBDI skanner).

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. Kui teie sõrmejälgede skannerit ei kuvata ja skanner on teie ARVUTISSE integreeritud, avage arvuti tootja veebisait. Otsige oma arvuti mudelist tehnilise toe jaotisest üles Windows 10 draiver skannerile, mida saate installida.

6. Kui skanner on PC-arvutist eraldi (lisatud USB kaudu), avage skanneri tootja veebisait, et otsida ja installida Windows 10 seadme draiveri tarkvara teie skanneri mudeli jaoks.
