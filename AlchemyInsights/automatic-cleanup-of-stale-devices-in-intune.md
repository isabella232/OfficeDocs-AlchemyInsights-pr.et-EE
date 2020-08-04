---
title: Aegunud seadmete automaatne puhastamine intunes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554965"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Aegunud seadmete automaatne puhastamine intunes

Intune võimaldab administraatoril seadistada ajaintervalli vahemikus 90 ja 270 päeva, pärast mida aegunud seadmed teenusest eemaldatakse. See säte on kogu organisatsioonis ja kui aktiveeritud, jõustub kohe. Kõik seadmed, mida pole Intune ' i serverile üle vaadatud, kustutatakse jäädavalt.

**Märkus** Ainult MDM-seadme objektid vastavad selle Kettapuhastuse toimingu tingimustele. Ainult EAS-i seadme objektid on välistatud.

Lisateavet selle kohta, millal seade saab seadme puhastamise sätete ja selle oleku alusel kustutamise tingimustele vastavaks, tehke järgmist.

Säte: **seadmete kustutamine pärast viimast sisseregistreerimise kuupäeva: Jah (teatud väärtused (N) määratud päevade lõikes)**

- Määratud väärtuse (N) põhjal, kui säte on konfigureeritud, kustutab Intune seadme määratud päevade jooksul pärast selle viimase edukat kontrollimist.

Säte: **seadmete kustutamine pärast viimast sisseregistreerimise kuupäeva: ei**

- 180 päeva pärast seadme serdi aegumist ja seda ei pikendata, kustutatakse seade.

**Märkus** Mõlemal juhul tuleb seade Intune ' is edukalt registreerida. Registreerimine toimub esimese seadme sissemöllimine ja Intune ' i teenusega.

Kui seade registreerib edukalt Intune ' i, kuid ei saanud Intune ' i registreerida, kustutatakse seade 270 päeva pärast registreerimist. (90 päeva, et märkida seade tühistatuks ja seejärel teine 180 päeva kirje kustutamiseks.)

Ühtegi mehhanismi pole praegu Intune ' i konsoolis, et tuvastada seadme sertide kehtivuse lõppkuupäev.