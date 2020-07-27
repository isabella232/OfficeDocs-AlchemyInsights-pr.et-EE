---
title: Intune ' i aktiveerimise lukustus juhendatud iOS-i seadmetes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423730"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Intune ' i aktiveerimise lukustus juhendatud iOS-i seadmetes

IOS-i seadmetes aktiveerimise lukustusest loobumise võimalus hõlbustab stsenaariumist taastumist, kui kasutaja lubab aktiveerimise lukustuse ettevõtte seadmes ja seejärel lahkub ettevõttest.

Aktiveerimise lukustusest möödumiseks on eeltingimused järgmised.

- Seade on "järelevalve all".
- Aktiveerimise lukustus on edukalt lubatud, kasutades iOS-i seadme piiramise poliitikat Intune ' is.

Lisaks peaksite aktiveerimise lukustusest loobumisel tegema järgmist.

- Seadme tühjendamine füüsiliselt.
- Kopeerige kood enne pühi väljastamist.

**Märkus:** Pühkige kood ei ole tõstutundlik, seega pole märke "-" ei nõuta.

Lisateavet leiate teemast [aktiveerimise lukustuse tühistamine iOS-i seadmetes, kus on Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**KKK**

K: **ma väljastasin serveri toimingu, et eemaldada seadmest ettevõtte andmed ja nüüd on see ootel olekus kinni.**

V: serveri toimingu edukaks lõpuleviimiseks peab sihipärane seade olema võrgus ja terve. Järgmistes olukordades jääb kaugprotseduurikutse 30 päevaks ootel olekusse või ajani, kui seade on seadme kinnitanud.

- Pole ühendust.
- Kaotab oma juhtimise oleku Intune ' iga.

Kui arvate, et seade ei ole enam sisse möllitud ja et see ei eemalda ettevõtte andmeid, valige Kustuta. Kustutamine eemaldab seadme kirje nii, et seda ei kuvata enam seadmete loendis. Kui soovite, et seade saaks uuesti aktiivseks, peab selle kasutaja seadme uuesti registreerima.

K: **miks pole teatud serveri toimingud minu jaoks saadaval?**

V: kõik platvormid ei toeta kõiki serveri seadme toiminguid. Järgmised Remote-toimingud on platvormile omased.

- Ümbersõit Activation Lock (ainult iOS)
- Värske algus (ainult Windows)
- Lost Mode (ainult iOS)
- Seadme leidmine (ainult iOS)
- Taaskäivita (ainult Windows)

Iga toimingu kohta leiate lisateavet teemast [Saadaolevad seadme toimingud](https://docs.microsoft.com/intune/device-management#available-device-actions).