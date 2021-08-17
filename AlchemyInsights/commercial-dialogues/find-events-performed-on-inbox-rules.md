---
title: Sisendkaustareeglitega seotud sündmuste korraldamine
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882631"
---
# <a name="find-events-performed-on-inbox-rules"></a>Sisendkaustareeglitega seotud sündmuste korraldamine

Kui sisendkausta reeglid luuakse, muudetakse või kustutatakse, salvestatakse sündmused auditilogisse. Nende läbivaatamiseks on vaja teha nii.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> **Audit**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Kui näete teadet, et peate auditeerimise sisse lülitama, lülitage see kohe sisse. Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.

2. Konfigureerige  lehe **Audit vahekaardil Otsing** järgmised sätted.
   - **Kuupäeva- ja kellaajavahemik:** valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - **Tegevused:** **valige suvand Uus sisendkaustReegel Loo sisendkausta** Outlook Web App

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Üksikasjade hüpiku avamiseks valige tulemitest soovitud tegevus. Jaotises **Parameetrid** näete reegli nime, tingimuste komplekti ja toiminguid, mida reegel teeb.

Lisateavet leiate teemast [Auditilogist otsimine, et uurida levinumaid tugiteenuseprobleeme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
