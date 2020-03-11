---
title: Sõrmejälje avamise suvandi kasutamine Windows 10-s
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588312"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Sõrmejälje avamise suvandi kasutamine Windows 10-s

**Luba Windows Hello sõrmejälg**

Windows 10 avamiseks sõrmejälje abil peate seadistama Windows Hello sõrmejälje, lisades (lastes Windowsil seda ära tunda) vähemalt üks sõrm. 

1. Avage **sätted > kontod > Sisselogimissuvandid** (või klõpsake [siin](ms-settings:signinoptions?activationSource=GetHelp)). Saadaolevad Sisselogimissuvandid loetletakse. Näiteks.

    ![Sisselogimissuvandid.](media/sign-in-options.png)

2. Klõpsake või koputage **Windows Hello sõrmejälg**, seejärel klõpsake nuppu **Seadista**. Klõpsake aknas Windows Hello häälestus **nuppu Alusta.** Sõrmejäljeandur aktiveeritakse ja teil palutakse panna sõrm sensoril:

   ![Sõrmejälje andur.](media/fingerprint-sensor.png)

3. Järgige juhiseid, mis palub teil oma sõrme korduvalt skannida. Kui see on lõppenud, on teil võimalus lisada muid sõrmi, mida võiksite sisselogimiseks kasutada. Järgmine kord, kui logite sisse Windows 10, on teil võimalus kasutada oma sõrmejälg seda teha.

**Windows Hello sõrmejälg pole sisselogimissuvandiga saadaval**

Kui Windows Hello sõrmejälge ei kuvata **Sisselogimissuvandite**suvandiga, tähendab see, et Windows ei tea ühtegi teie arvutiga ühendatud sõrmejäljelugejat/skannerit või süsteemipoliitika takistab selle kasutamist (nt teie arvuti haldab teie töökoht). Tõrkeotsingu sooritamiseks toimige järgmiselt. 

1. Valige tegumiribal nupp **Start** ja otsige **seadmehaldurit**.

2. Klõpsake või koputage **Seadmehalduri**avamiseks.

3. Laiendage Seadmehalduris biomeetrilisi seadmeid, klõpsates selle glüüfi.

   ![Biomeetrilised seadmed.](media/biometric-devices.png)

4. Sõrmejäljelugeja tuleks loetleda biomeetrilise seadena (nt Synaptics WBDI skanner):

   ![Biomeetrilised seadmed.](media/biometric-devices-expanded.png)

5. Kui sõrmejäljelugeja ei kuvata ja skanner on arvutisse integreeritud, arvuti tootja veebisaidile. Otsige oma arvuti mudeli tehnilise toe sektsioonis üles Windows 10 draiver skanneri jaoks, mida saate installida.

6. Kui skanner on ARVUTIST eraldi (manustatud USB kaudu), skanneri tootja veebisaidile, et leida ja installida Windows 10 seadmedraiveri tarkvara teie skanneri mudelile.
