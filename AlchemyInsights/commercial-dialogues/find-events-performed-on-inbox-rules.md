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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313495"
---
# <a name="find-events-performed-on-inbox-rules"></a>Sisendkaustareeglitega seotud sündmuste korraldamine

Kui sisendkausta reeglid luuakse, muudetakse või kustutatakse, salvestatakse sündmused auditilogisse. Nende läbivaatamiseks on vaja teha nii.

1. Tehke ühte järgmistest toimingutest.
   - Avage Microsoft 365 vastavuskeskus lahenduste audit <https://compliance.microsoft.com>  \> . Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://compliance.microsoft.com/auditlogsearch> .
   - Avage Microsoft 365 Defender , valige <https://security.microsoft.com> **Auditeeri**. Või otse lehele Auditeeri **minemiseks** kasutage funktsiooni <https://security.microsoft.com/auditlogsearch> .

    **Märkus.** Kui näete teadet, et peate auditeerimise sisse lülitama, lülitage see kohe sisse. Kui see funktsioon pole sisse lülitatud, ei saa otsingutulemid eelmistest kuupäevadest andmeid tõmmata.
1. Valige väli Tegevused ja otsige üles Exchange ja seejärel valige New-InboxRule Loo sisendkausta reegel Outlook Web App. Kui olete lõpetanud, klõpsake paani Tegevused minimeerimiseks väljaspool paani.
1. Määrake kuupäevavahemik ja seejärel valige väljal Kasutajad selle kasutaja kasutajanimi, mida soovite uurida. Korraga saate valida mitu kasutajat.
1. Valige Otsi. Tegevused kuvatakse jaotises Tulemid.
1. Üksikasjade kuvamiseks valige soovitud tegevus ja seejärel valige Lisateave. Jaotises Parameetrid näete reegli nime, tingimuste komplekti ja toiminguid, mida reegel teeb.

2. Konfigureerige  lehe **Audit vahekaardil Otsing** järgmised sätted.
   - **Kuupäeva- ja kellaajavahemik:** valige väljadele Algus ja Lõpp **kuupäeva-/kellaajavahemik.** 
   - **Tegevused:** **valige suvand Uus sisendkaustReegel Loo sisendkausta** Outlook Web App

3. Kui olete lõpetanud, klõpsake nuppu **Otsi**. Tegevused kuvatakse uuel lehel **Auditiotsing.**

4. Üksikasjade hüpiku avamiseks valige tulemitest soovitud tegevus. Jaotises **Parameetrid** näete reegli nime, tingimuste komplekti ja toiminguid, mida reegel teeb.

Lisateavet leiate teemast [Auditilogist otsimine, et uurida levinumaid tugiteenuseprobleeme.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
