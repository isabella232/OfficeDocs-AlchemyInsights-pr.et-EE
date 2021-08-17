---
title: 1491-search-not-returning-expected-results
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052706"
---
# <a name="content-search-not-returning-expected-results"></a>Sisuotsing ei tagasta oodatud tulemusi

Kui käivitate sisuotsinguid Microsoft 365 turbe- &, võidakse kuvada ootamatud otsingutulemid. Kaaluge järgmisi asju, mis võivad teie otsingutulemeid mõjutada.

- **Sisu asukohad ja otsingutingimused.** Veenduge, et olete valinud õiged sisukohad ja otsingutingimused. Kui käivitate suure otsingu (paljude asukohtadega), kaaluge selle tükeldamist mitmeks otsinguks.

- **Osaliselt indekseeritud üksused.** Postkastide osaliselt  [indekseeritud](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) üksused kaasatakse hinnanguliste otsingutulemite hulka. Küll aga ei kaasata otsinguhinnangusse SharePoint OneDrive saitidelt pärit osaliselt indekseeritud üksusi.

- **Otsingutõrked.** Kui otsite suurt hulka postkaste (üle 100 000 postkasti), võidakse kuvada otsingutõrkeid, mille tõrkekoodid on näiteks CS008-009 ja CS012-002). Sel juhul tuleb uuesti otsida ainult nurjunud sisuasukohti. Lisateavet  [leiate sellest](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) artiklist.
