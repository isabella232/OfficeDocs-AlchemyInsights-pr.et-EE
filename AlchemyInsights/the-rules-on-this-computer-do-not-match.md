---
title: Tõrge. Selles arvutis kehtivad reeglid ei vasta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782948"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Tõrge. Selles arvutis kehtivad reeglid ei vasta

Teadaoleva probleemi värskendatud oleku kuvamiseks lugege teemat Selle arvuti reeglid ei [vasta Microsoft Exchange'i reeglitele.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlooki meeskond on rakendanud paranduse järgus 12928.10000. Lahendus on juba Insider Fastis ja see läheb kuupõhisele kanalile juuni lõpus 2020. Kui olete fikseeritud järgu saanud, võidakse teil viimast korda kuvada viip "Milliseid reegleid soovite säilitada". Kui teilt küsitakse, valige Server ja seejärel minge Outlookis tagasi ja lubage uuesti kõik keelatud reeglid.

Kuni parandus on saadaval, kasutage järgmist lahendust.

**Lahendus.** Hiljutistes aruannetes ilmnes probleem nende jaoks, kes on outlooki töölauarakenduses loonud ainult kliendireeglid. Kui probleem ei lahene, kaaluge reeglite kustutamist ning seejärel looge ja redigeerige reegleid ainult OWA-s (Outlook Web Appis), kuni probleem on lahendatud.

Kui te ei saa reegleid käsitsi kustutada, saate Outlooki käivitamisel käivitada Outlooki käsu, käivitades Outlook.exe /cleanrules. See kustutab nii kliendi- kui ka serverireeglid. See kustutab kõik Outlooki profiili kõigi kontode reeglid. See käsk on veel dokumenteeritud artiklis Käsurealülitid.

