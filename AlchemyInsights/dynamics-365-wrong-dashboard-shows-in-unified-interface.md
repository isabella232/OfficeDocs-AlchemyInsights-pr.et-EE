---
title: Dynamics 365 – vale armatuurlaud kuvatakse rakenduses Dynamics 365 Unified Interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711271"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Rakenduses Dynamics 365 Unified Interface kuvatakse valed armatuurlauad

On mitu põhjust, miks võidakse kuvada mõni muu armatuurlaud kui see, mida ootate.

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kasutaja on määranud kasutaja vaike-armatuurlaua. 

Tavaliselt saate määrata kasutaja vaike-armatuurlaua, kui nupp **Sea vaikesätteks** ei kuvata armatuurlaual. Kasutaja vaike-armatuurlaud alistab kõik muud vaike-armatuurlauad, isegi kui kasutaja vaike-armatuurlaud pole praeguses rakenduses.

Kasutage järgmisi lahendusi, et Andmebaasiparooli tühistamine nende vaike-armatuurlaud.

1. Saate luua uue isikliku armatuurlaua.

2. Seadke uus armatuurlaud kasutaja vaikesätteks.

3. Armatuurlaua kustutamine.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Armatuurlaud on määratud sitemap-s

Võimalik, et olete määranud organisatsiooni vaike-armatuurlaua, valides armatuurlaua ja valides jaotises "süsteemi kohandamine" valiku "Määra vaikesätteks". Kui kasutajal on juurdepääs sellele armatuurlauale, on sisukaarti kujundajas määratletud armatuurlaud ülimuslikud.

Kui soovite, et kasutajad näeksid armatuurlauda, mille olete määranud organisatsiooni vaikeprogrammiks, saate teha järgmist.

* Armatuurlaua seadmine sisukorda

* Juurdepääsu eemaldamine nende kasutajate jaoks mõeldud sitemap-i jaoks määratud armatuurlauale
