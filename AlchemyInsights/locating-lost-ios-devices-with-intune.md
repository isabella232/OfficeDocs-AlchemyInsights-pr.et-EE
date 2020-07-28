---
title: Kaotsiläinud iOS-i seadmete leidmine Intune ' i abil
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439144"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Kaotsiläinud iOS-i seadmete leidmine Intune ' i abil

IOS-i seadmes kaotatud režiimi lubamine võimaldab administraatoril kuvada lukustuskuval sõnumi ja kontaktisiku telefoninumbri.

Pärast kaotatud režiimi lubamist saab administraator kasutada seadme asukoha tuvastamiseks seadme asukohta.

Seadme asukoha tuvastamine Intune ' is töötab koos iOS-i seadmetega, et kuvada kindla seadme asukoht kaardil.

Selle toimingu kasutamiseks peab iOS-i seade olema:

- Juhendav režiim
- Kaotatud režiim

Lisateavet leiate teemast [kaotsiläinud režiimi lubamine iOS-i/iPadOS seadmetes, kus](https://docs.microsoft.com/intune/device-lost-mode) on Intune ' is kaotatud [või varastatud iOS-i/iPadOS seadmete otsimine](https://docs.microsoft.com/intune/device-locate).

**KKK**

K: ma väljastasin serveri toimingu, et eemaldada seadmest ettevõtte andmed ja nüüd on see ootel olekus kinni.

V: serveri toimingu edukaks lõpuleviimiseks peab sihipärane seade olema võrgus ja terve. Järgmistes olukordades jääb kaugprotseduurikutse 30 päevaks ootel olekusse või ajani, mil seade selle käsu kinnitab.

- Kui seadmel pole ühenduvust
- Kui seade kaotab oma juhtimise oleku Intune ' iga

Kui arvate, et seade ei kontrolli enam ja et see ei saa ettevõtte andmeid eemaldada, valige Kustuta. Kustutamine eemaldab seadme kirje nii, et seda ei kuvata enam seadmete loendis. Kui seade muutub taas aktiivseks, peab selle kasutaja selle uuesti registreerima.

K: Miks pole teatud serveri toimingud minu jaoks saadaval?

V: kõik platvormid ei toeta kõiki serveri seadme toiminguid. Järgmised serveri toimingud on platvormile omased, nii et need on saadaval ainult nende platvormide jaoks, mida on märgitud.

- Ümbersõit Activation Lock (ainult iOS)
- Värske algus (ainult Windows)
- Lost Mode (ainult iOS)
- Seadme leidmine (ainult iOS)
- Taaskäivita (ainult Windows)

Iga toimingu kohta leiate lisateavet teemast [Saadaolevad seadme toimingud](https://docs.microsoft.com/intune/device-management#available-device-actions).