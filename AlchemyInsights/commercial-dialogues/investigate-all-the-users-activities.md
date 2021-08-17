---
title: Kõigi kasutajate tegevuste uurimiseks
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898792"
---
# <a name="investigate-all-the-users-activities"></a>Kõigi kasutajate tegevuste uurimiseks

Selleks tehke nii.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste <https://compliance.microsoft.com>  \> **audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Kui märkate, et peate funktsiooni sisse lülitama, lülitage see kohe sisse. Kui funktsioon pole sisse lülitatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.

2. Konfigureerige  lehe **Audit vahekaardil Otsing** järgmised sätted.
   - **Kuupäeva- ja kellaajavahemik:** valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - **Tegevused.** Kui olete huvitatud konkreetsest tegevusest, valige see loendist; muul juhul tagastab vaikeväärtus **Kuva kõigi tegevuste tulemid** kõik tegevused.
   - **Kasutajad:** aktsepteerige kõigi kasutajate tulemite tagastamiseks tühi vaikeväärtus või sisestage üks või mitu kasutajat.

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.** Näete **IP-aadressi,** kasutaja **ja** **tegevuse** nime.

4. Tulemite allalaadimiseks valige Ekspordi **alla** \> **kõik tulemid**.

5. Üksikasjade hüpiku avamiseks valige tulemitest soovitud tegevus.

Lisateavet leiate teemast [Auditilogist otsimine, et uurida levinumaid tugiteenuseprobleeme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
