---
title: Microsoft Defenderi Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330056"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Microsoft Defenderi Office 365

Siin on mõned lahendused levinud probleemidele Microsoft Defenderi Office 365.

- **Sõnumi viivitus:**

  Meilisõnumite kohaletoimetamise viivitused võivad olla seif manuste skannimine. Lisateavet leiate teemast [seif Manuste poliitikasätted](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Väärpositiivsetest või negatiivsetest tulemustest teatamine**

  Lisateavet leiate teemast [Sõnumitest ja failidest teatamine Microsoftile.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Luba seif linkide kaitse:**

  1. Avage Microsoft 365 Defender portaal jaotises Poliitikad <https://security.microsoft.com/> **& Meilipoliitikad** & Reeglid \>  \>  \> **ohupoliitikad seif** **Lingid.**

     Otse lehele Lingid **seif kasutage** . <https://security.microsoft.com/safelinksv2>

  2. Valige **seif linkide** lehel poliitika, klõpsates poliitika nime.
  3. Tehke kuvatavas üksikasja hüpikmenüüs ühte järgmistest toimingutest.
     - Uue poliitika lisamiseks valige **+ Loo**. Poliitikasätete määratlemiseks käivitatakse viisard.
     - Olemasoleva poliitika redigeerimiseks valige poliitika, klõpsates poliitika nime. Klõpsake kuvatavas üksikasja hüpikmenüüs **jaotises Kaitsesätted** **nuppu** Redigeeri.
  4. Konfigureerige **lehel** Kaitsesätted järgmised sätted.
     - Lülitage **sisse suvand Valige sõnumites tundmatute potentsiaalselt pahatahtlike URL-ide jaoks toiming.**
     - Valige **Rakenda ettevõttes saadetud sõnumitele turvalised lingid.**

  Lisateavet leiate teemast Microsoft [Defenderi seif linkide poliitikate](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)Office 365.
