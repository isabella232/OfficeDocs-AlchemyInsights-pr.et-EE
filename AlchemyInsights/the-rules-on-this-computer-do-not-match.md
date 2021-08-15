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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981109"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Tõrge. Selles arvutis kehtivad reeglid ei vasta

Teadaoleva probleemi värskendatud oleku kuvamiseks lugege teemat Selle arvuti reeglid ei vasta Microsoft [Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook on rakendanud paranduse järgus 12928.10000. Lahendus on juba Insider Fastis ja see läheb kuupõhisele kanalile juuni lõpus 2020. Kui olete fikseeritud järgu saanud, võidakse teil viimast korda kuvada viip "Milliseid reegleid soovite säilitada". Kui küsitakse, valige Server ja seejärel minge tagasi Outlook ja lubage uuesti kõik keelatud reeglid.

Kuni parandus on saadaval, kasutage järgmist lahendust.

**Lahendus.** Hiljutistes aruannetes ilmnes probleem nende jaoks, kes on loonud ainult Outlook klientrakenduse reeglid. Kui probleem ei lahene, kaaluge reeglite kustutamist ning seejärel looge ja redigeerige reegleid ainult OWA-s (Outlook Web App), kuni probleem on lahendatud.

Kui te ei saa reegleid käsitsi kustutada, saate käivitada Outlook käsu, kui käivitate Outlook käivitades Outlook.exe /cleanrules. See kustutab nii kliendi- kui ka serverireeglid. See kustutab kõik reeglid kõigi kontoreeglite Outlook. See käsk on veel dokumenteeritud artiklis Käsurealülitid.

