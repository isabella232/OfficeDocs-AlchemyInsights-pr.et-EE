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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003385"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Luba päranddialoogide kinnitamine aruannete avamiseks

**Sümptom**

Kasutajad ei saa aruandeid avada. "Midagi on valesti läinud. Lisateabe saamiseks vaadake tehnilisi üksikasju."

**Põhjus**

Aruannete laadimine UCI-s nurjub tõrkega "Vormideskriptor on null või pole määratletud". Aruanded UCI-s vajavad siiski päranddialooge, nii et kliendi süsteem peab lubama *allowlegacydialogsembedding*.

**Lahendus**

1. Avage **Settings >Administration > System Settings > Vahekaart Üldine**.

2. Määrake väärtuse "Luba teatud päranddialoogide manustamine ühendatud kasutajaliidese brauserikliendis" väärtuseks **Jah**.
