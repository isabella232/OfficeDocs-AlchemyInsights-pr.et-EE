---
title: Windows 10 käivitamise sätted
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751131"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10 käivitamise sätted

**Käivitamisel automaatselt käivitatavate rakenduste muutmine**

1. Avage [sätted > rakendused > käivitus](ms-settings:startupapps?activationSource=GetHelp).

2. Veenduge **,** et mõni rakendus, mida soovite käivitamisel käitada, oleks sisse lülitatud.

**Rakenduse käivitamisel automaatselt käivitumiseks rakenduse lisamine**

1. Klõpsake või puudutage nuppu **Käivita** ja otsige üles rakendus, mille soovite käivitada käivitamisel.

2. Paremklõpsake rakendust, klõpsake käsku **rohkem**ja seejärel klõpsake käsku **Ava kausta asukoht**. Avaneb asukoht, kus rakenduse otsetee on salvestatud. Kui fail pole avatud, tähendab see seda, et rakendust ei saa käivitamisel käitada.

3. Kui faili asukoht on avatud, vajutage klahvikombinatsiooni **Windowsi logoga klahv + R**, tippige **Shell: Startup**ja seejärel klõpsake nuppu **OK**. Avatakse kaust Startup (Startup).

4. Kopeerige ja kleepige otsetee rakendusse, mis asub kaustast Startup (käivituskaustas).

**Täpsemad käivitamise suvandid (sh turvarežiim, UEFI sätted ja teisest seadmest käivitamine)**

1. Salvestage oma töö ja sulgege avatud dokumendid, kuna need toimingud taaskäivitavad teie arvuti.

2. Avage [sätted > värskenda & turve > taastamine](ms-settings:recovery?activationSource=GetHelp).

3. Klõpsake jaotises **Täpsem käivitamine**nuppu **Taaskäivita kohe**. 

4. Pärast arvuti taaskäivitamist valige Kuva valik.

    - Seadmest (nt USB-draivilt) buutimiseks klõpsake nuppu **Kasuta seadet**.

    - UEFI sätete (mõnikord BIOS-i häälestamise) sisestamiseks klõpsake nuppu **tõrkeotsing > Täpsemad suvandid > UEFI püsivara sätted**. 

    - Turvarežiimi sisestamiseks või täpsemate käivitamise sätete muutmiseks klõpsake nuppu **tõrkeotsing > Täpsemad suvandid > käivitamise sätted**ja seejärel klõpsake nuppu **Taaskäivita**. Teil võidakse paluda sisestada [BitLockeri taastevõti](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Kui teie arvuti taaskäivitub uuesti, klõpsake selle käivitamise säte, mida soovite kasutada.