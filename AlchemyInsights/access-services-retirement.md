---
title: Accessi teenuste kasutuselt kõrvaldamine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938691"
---
# <a name="access-services-retirement"></a>Accessi teenuste kasutuselt kõrvaldamine

Nagu me algselt mc97576's teada andsime, jätkasime 2017. aasta märtsis suhtlemist viimase aasta jooksul, Accessi teenused on pensionile jäänud. Selle protsessi järgmise etapina eemaldatakse Accessi veebiandmebaasid, mis kasutavad SharePoint nende aluseks olevat andmesalvestusruumi.

**Kuidas see mind mõjutab?**

Alates 2019. aasta juunist lõpetame SharePoint Online'is uute Accessi andmebaaside loomise ning sulgeme teenuse ja kõik ülejäänud rakendused 2020. aasta aprilliks.

**Mida on vaja selle muudatuse ettevalmistamine teha?**

Soovitame teil luua üleminekuplaani oma ettevõtte Accessi veebiandmebaaside jaoks. Administraatorid saavad [accessi SharePoint kasutada accessi](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) rakenduse skannerit, et hankida nende Accessi rakenduste inventuur, mida saidid kasutavad.

Accessi veebiandmebaaside andmete migreerimiseks on mitu võimalust.

- Importimine kohalikku Accessi andmebaasi (. ACCDB) või Excel faili.
- Samuti soovitame uurida Microsoft PowerApps platvormina, et luua veebi- ja mobiilsideseadmete jaoks koodita ärilahendusi.