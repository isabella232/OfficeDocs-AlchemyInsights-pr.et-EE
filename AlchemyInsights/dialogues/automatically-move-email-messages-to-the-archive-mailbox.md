---
title: Meilisõnumite automaatne ümberpaigutamine arhiivi postkasti
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525099"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Meilisõnumite automaatne ümberpaigutamine arhiivi postkasti

Siin on juhised selle kohta, kuidas häälestada poliitika kasutaja vana meili arhiivi postkasti automaatselt üle viima.

1. Valige [**turbe & nõuetele vastavuse**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **andmete haldamise**  >  **arhiivi** , et kontrollida, kas arhiivi postkast on kasutaja jaoks lubatud. Kui pole, klõpsake väljal hoiatus nuppu **Luba** ja siis nuppu **Jah** .
2. Avage [**Exchange ' i halduskeskus > nõuetele vastavuse haldus > säilituse sildid**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Valige ikoon + ja seejärel valige nupp **Rakenda automaatselt tervele postkastile**.
4. Määrake säilituse sildile nimi ja valige käsk **VII arhiivi**. Sisestage ooteaeg soovitud aeg (nt 90 päeva). Klõpsake nuppu **Salvesta**.
5. Nüüd looge säilituspoliitika: valige **säilituspoliitika**, valige uue poliitika lisamiseks ikoon.
6. Määrake säilituspoliitika nimi, seejärel klõpsake ja liikuge, et leida ja lisada äsja loodud säilituse silt. Klõpsake nuppu **Salvesta**.
7. Lõpuks rakendage säilituspoliitika kasutaja postkastile: endiselt Exchange ' i administreerimiskeskuses Avage **adressaadi**  >  **postkastid**. Valige kõik kasutajad, kellele soovite poliitika rakendada, ja seejärel valige käsk **Redigeeri** (pliiatsi ikoon).
8. Klõpsake dialoogiboksis nuppu **postkasti funktsioonid**. Rakendage jaotises **säilituspoliitika** selle poliitika, mille äsja lõite > **Salvesta**.
9. Juhised poliitika rakendamiseks kõigile kasutajatele leiate teemast [säilituspoliitika rakendamine postkastidele](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
