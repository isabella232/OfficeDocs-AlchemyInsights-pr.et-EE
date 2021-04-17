---
title: Windows 10 käivitussätted
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828148"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10 käivitussätted

**Käivituse ajal automaatselt käivituvate rakenduste muutmine**

1. Avage [Sätted > Rakendused > Käivitus](ms-settings:startupapps?activationSource=GetHelp).

2. Veenduge, et iga rakendus, mida soovite käivitamisel käitada, oleks sisse **lülitatud.**

**Rakenduse lisamine käivitumiseks automaatselt käivitamisel**

1. Klõpsake või **puudutage nuppu Start** ja otsige üles rakendus, mida soovite käivitamisel käivitada.

2. Paremklõpsake rakendust, klõpsake käsku **Rohkem** ja seejärel klõpsake käsku **Ava faili asukoht.** See avab asukoha, kuhu rakenduse otsetee salvestatakse. Kui faili asukoha avamiseks pole valikut, tähendab see, et rakendust ei saa käivitamisel käivitada.

3. Kui faili asukoht on avatud, vajutage klahvikombinatsiooni **Windowsi logoga klahv + R**, tippige **shell:startup** ja seejärel klõpsake nuppu **OK**. Avatakse käivituskaust.

4. Kopeerige ja kleepige rakenduse otsetee faili asukohast käivituskausta.

**Täpsemad käivitussuvandid (sh turvarežiim, UEFI sätted ja käivitamine teisest seadmest)**

1. Salvestage oma töö ja sulgege kõik avatud dokumendid, kuna need toimingud taaskäivitavad teie arvuti.

2. Avage [Sätted > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Klõpsake **jaotises Täpsem käivitus** nuppu Taaskäivita **kohe**. 

4. Pärast arvuti taaskäivitamist kuvale Suvandi valimine tehke valik.

    - Seadmest (nt USB-draivilt) algkäivituseks klõpsake **nuppu Kasuta seadet**.

    - UEFI sätete (mõnikord nimetatakse seda ka BIOS-i häälestuseks) sisestamiseks klõpsake **> Täpsemad suvandid > UEFI püsivarasätted**. 

    - Turvarežiimi sisenemiseks või täpsemate käivitussätete muutmiseks klõpsake nuppu **Tõrkeotsing > Täpsemad suvandid >** Ja seejärel klõpsake nuppu **Taaskäivita**. Teil võidakse paluda sisestada [BitLockeri taastevõti.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Pärast arvuti taaskäivitamist klõpsake käivitussätet, mida soovite kasutada.