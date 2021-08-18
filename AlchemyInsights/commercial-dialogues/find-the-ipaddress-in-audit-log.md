---
title: IP-aadressi otsige auditilogist
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902256"
---
# <a name="find-the-ip-address-in-audit-log"></a>IP-aadressi otsige auditilogist

Ip-aadress, mis vastab kasutaja või administraatori tegevusele, kuvatakse auditilogides. Klienditeave logitakse ka. IP-aadressi tuvastamiseks tehke nii.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Kui näete teadet, et peate auditeerimise sisse lülitama, lülitage see kohe sisse. Kui see funktsioon pole lubatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.

2. Kontrollige **lehel** Audit, kas vahekaart **Otsing** on valitud, ja seejärel konfigureerige järgmised sätted.
   - **Kuupäeva- ja kellaajavahemik:** valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - **Tegevused.** Kui olete huvitatud konkreetsest tegevusest, valige see loendist; vastasel korral tagastatakse vaikeväärtus **Kuva kõigi tegevuste** tulemid kõik tegevused. Arvestage, et teatud tegevused ei pruugi valiku jaoks saadaval olla; Kui valitud on kõigi tegevuste tulemite **kuvamine, tagastatakse need** auditiüksused.
   - **Kasutajad:** aktsepteerige kõigi kasutajate tulemite tagastamiseks tühi vaikeväärtus või sisestage üks või mitu kasutajat.

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Klõpsake tulemite väljal **Filtreeri tulemeid** ja tippige **väljale Tegevuse** filter käsk Sea postkast.

5. Valige tulemitest auditikirje, et avada hüpik **Üksikasjad.**

Lisateavet leiate teemast [Auditilogist otsimine, et uurida levinumaid tugiteenuseprobleeme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
