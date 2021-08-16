---
title: Dynamics 365 – vale armatuurlaua kuvab Dynamics 365 unified Interface'is
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101478"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Vale armatuurlaud kuvatakse Dynamics 365 ühtses liideses

On mitu põhjust, miks võidakse kuvada mõni muu armatuurlaud kui see, mida ootate.

## <a name="the-user-has-set-a-user-default-dashboard"></a>Kasutaja on määranud kasutaja vaikearmatuurlaua 

Tavaliselt saate tuvastada, et kasutaja vaikearmatuurlaud määratakse siis, kui armatuurlaua käsuribal nuppu Sea vaikeväärtuseks ei näidata.  Kasutaja vaikearmatuurlaud alistab kõik muud vaikearmatuurlauad, isegi kui kasutaja vaikearmatuurlaud pole praeguses rakenduses.

Vaikearmatuurlaua lähtestamiseks kasutage järgmist lahendust.

1. Looge uus isiklik armatuurlaud.

2. Määrake uus armatuurlaud kasutaja vaikearmatuurlauaks.

3. Kustutage see armatuurlaud.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Armatuurlaud on määratud saidikaardil

Võimalik, et olete määranud organisatsiooni vaikearmatuurlaua, valides armatuurlaua ja valides jaotises "Süsteemi kohandamine" käsu Sea vaikesaks. Kuid saidikaardi kujundajas määratletud armatuurlaud on selle armatuurlaua ees ülimuslik, kui kasutaja pääseb sellele juurde.

Kui soovite, et kasutajad näeks armatuurlauda, mille olete määranud ettevõtte vaikearmatuurlauaks, saate teha ühte järgmistest.

* Armatuurlaua määramine saidikaardil

* Nende kasutajate jaoks saidikaardi määratletud armatuurlauale juurdepääsu eemaldamine
