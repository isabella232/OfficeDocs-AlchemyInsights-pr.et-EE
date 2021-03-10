---
title: Täpsemate jahipidamise päringute heade tavade rakendamine
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694269"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Täpsemate jahipidamise päringute heade tavade rakendamine

Tulemuste kiiremaks ja ajalõpute vältimiseks keerukate päringute käitamise ajal rakendage järgmisi häid tavasid.

- Kui proovite uusi päringuid, kasutage alati limiiti, et vältida väga suurte tulemite tekkimist. Samuti saate `count` määrata tulemikomplekti suuruse esialgse hinnangu.
- Kasutage kõigepealt ajafiltreid. Ideaaljuhul Piirake päringuid seitsme päevaga.
- Lisage päringu alguses kohe pärast filtrit soovitud filtrid, et enamik andmeid eemaldada.
- Kui otsite täielikke märke, kasutage `has` tehtemärki mitte `contains` .
- Saate otsida kindla veeru otsinguid, mitte kõigis veergudes.
- Tabelitega liitumisel Määrake esmalt tabel, kus on vähem ridu.
- `project` ainult teie liitunud tabelite vajalikud veerud.

Lisateavet leiate teemast [täiustatud jahi päringu parimad tavad](https://go.microsoft.com/fwlink/?linkid=2144812).
