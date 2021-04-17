---
title: Luba päranddialoogide kinnitamine aruannete avamiseks
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814260"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Luba päranddialoogide kinnitamine aruannete avamiseks

**Sümptom**

Kasutajad ei saa aruandeid avada. "Midagi on valesti läinud. Lisateabe saamiseks vaadake tehnilisi üksikasju."

**Põhjus**

Aruannete laadimine UCI-s nurjub tõrkega "Vormideskriptor on null või pole määratletud". Aruanded UCI-s vajavad siiski päranddialooge, nii et kliendi süsteem peab lubama *allowlegacydialogsembedding*.

**Lahendus**

1. Avage **Settings >Administration > System Settings > Vahekaart Üldine**.

2. Määrake väärtuse "Luba teatud päranddialoogide manustamine ühendatud kasutajaliidese brauserikliendis" väärtuseks **Jah**.
