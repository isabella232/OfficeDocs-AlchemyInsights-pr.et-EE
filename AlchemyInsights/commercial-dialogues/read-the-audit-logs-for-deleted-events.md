---
title: Kustutatud sündmuste auditilogide lugemine
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896011"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Kustutatud sündmuste auditilogide lugemine

Selleks tehke nii.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Kui märkate, et peate funktsiooni sisse lülitama, lülitage see kohe sisse. Kui funktsioon pole sisse lülitatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.

2. Konfigureerige  lehe **Audit vahekaardil Otsing** järgmised sätted.
   - **Kuupäeva- ja kellaajavahemik:** valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - **Tegevused:** **sisestage Exchange ja** seejärel valige järgmised väärtused.
     - **Kustutatud sõnumid kaustast Kustutatud üksused**
     - **Teisaldatud sõnumid kausta Kustutatud üksused**

       Kui olete lõpetanud, klõpsake paani Tegevused minimeerimiseks väljaspool **paani.**

   - **Kasutajad:** aktsepteerige kõigi kasutajate tulemite tagastamiseks tühi vaikeväärtus või sisestage üks või mitu kasutajat.

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Üksikasjade hüpiku avamiseks valige tulemitest soovitud tegevus. Lisateavet kustutatud üksuse kohta (nt teemarida ja üksuse asukoht kustutamisel) kuvatakse väljal **AffectedItems.**

   > [!NOTE]
   > Kustutatud üksusi ei saa auditilogi funktsiooni abil taastada. Kustutatud üksuste taastamiseks lugege teemat [Kustutatud meilisõnumite taastamine Outlooki veebirakendus](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Lisateavet leiate teemast [Auditilogist otsimine, et uurida levinumaid tugiteenuseprobleeme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
