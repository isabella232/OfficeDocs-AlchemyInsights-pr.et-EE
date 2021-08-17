---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105564"
---
# <a name="troubleshoot-content-search-errors"></a>Sisuotsingu tõrgete tõrkeotsing

Kas teil on probleeme sisuotsinguga või saate otsingutulemite eksportimisel tõrkeid?

Näiteks kas otsingute käivitamisel kuvatakse järgmine tekst?

- CS008 või CS012 tõrked

- Serveri hõivatud/ajalõpu tõrked

- Ilmnes rakenduse tõrge

Või kui otsite või ekspordite tulemeid suurest arvust postkastidest (üle 100 000 postkasti), kas saate eksporditõrkeid?

Seda tüüpi tõrgete korral saate uuesti otsida nurjunud sisuasukohti. Lisateavet  [leiate sellest](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) artiklist.

Kui ekspordite rohkem kui 100 K postkasti, peate tulemite eksportimiseks kasutama järgmist PowerShelli: tulemite eksportimine rohkem kui [100K postkastidest.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)
