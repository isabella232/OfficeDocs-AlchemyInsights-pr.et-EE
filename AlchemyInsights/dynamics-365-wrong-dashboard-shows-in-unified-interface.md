---
title: Dynamics 365-vale armatuurlaud näitab Dynamics 365 ühendatud liides
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528547"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Vale armatuurlaud näitab Dynamics 365 ühendatud liides

On mitu põhjust, miks võite näha teise armatuurlaua kui see, mida ootate:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kasutaja on seadnud kasutaja vaikimisi armatuurlaud 

Tavaliselt saate tuvastada kasutaja vaikimisi armatuurlaud on seatud kui vaikimisi nuppu **Sea** ei kuvata armatuurlaua käsuribal. Kasutaja vaikimisi armatuurlaud alistab kõik muud vaikimisi armatuurlauad isegi siis, kui kasutaja vaikimisi armatuurlaud ei ole praeguses rakenduses.

Kasutage järgmist lahendust, et Tühista oma vaikimisi armatuurlaud.

1. Saate luua uue isikliku armatuurlaua.

2. Seadke see uus armatuurlaud kasutaja vaikesätteks.

3. Kustutage armatuurlaud.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Armatuurlaud on seatud saidikaardi

Võimalik, et olete seadistanud organisatsiooni vaike-armatuurlaua, valides armatuurlaua ja valides jaotises "Kohanda süsteemi". Kuid saidikaardi kujundajas määratletud armatuurlaud on selle armatuurlaua suhtes ülimuslik, kui kasutajal on sellele juurdepääs.

Kui soovite, et kasutajad näeksid armatuurlauda, mille olete seadnud organisatsiooni vaikesätteks, saate teha järgmist:

* Armatuurlaua seadmine saidikaardi

* Eemalda juurdepääs saidikaardi määratud armatuurlauale nende kasutajate jaoks
