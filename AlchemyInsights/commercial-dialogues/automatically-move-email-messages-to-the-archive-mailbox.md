---
title: Meilisõnumite automaatne teisaldamine arhiivipostkasti
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
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059222"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Meilisõnumite automaatne teisaldamine arhiivipostkasti

Poliitika häälestamiseks kasutaja vana meilisõnumi automaatseks teisaldamiseks arhiivipostkasti on järgmine.

1. Kasutaja [**jaoks on & arhiivipostkasti**](https://go.microsoft.com/fwlink/p/?linkid=2077143)kontrollimiseks avage turbe- ja  >    >   vastavusandmete haldamise arhiivimine. Kui seda pole, klõpsake **hoiatusväljal** **nuppu Luba** ja siis nuppu Jah.
2. Avage [**Exchange halduskeskus > säilitussiltide > haldus.**](https://go.microsoft.com/fwlink/?linkid=2059104)
3. Valige ikoon + ja seejärel valige **kogu postkastile automaatselt rakendav ikoon**.
4. Määrake säilitussildile nimi ja valige **Teisalda arhiivi.** Sisestage säilitusperioodi jaoks soovitud aeg (nt 90 päeva). Klõpsake nuppu **Salvesta**.
5. Nüüd looge säilituspoliitika: valige **säilituspoliitikad** ja valige uue poliitika lisamiseks ikoon.
6. Määrake säilituspoliitikale nimi, klõpsake ja liikuge kerides äsja loodud säilitussildi otsimiseks ja lisamiseks. Klõpsake nuppu **Salvesta**.
7. Lõpuks rakendage säilituspoliitika kasutaja postkastile: avage endiselt Exchange halduskeskuses   >  **adressaadipostkastid.** Valige kõik kasutajad, kellele soovite poliitika rakendada, ja seejärel valige **Redigeeri** (pliiatsiikoon).
8. Klõpsake dialoogiboksis nuppu **Postkastifunktsioonid.** Rakendage **jaotises Säilituspoliitika** äsja loodud poliitika > **Salvesta**.
9. Juhised poliitika rakendamiseks kõigile kasutajatele leiate teemast [Säilituspoliitika rakendamine postkastidele.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
