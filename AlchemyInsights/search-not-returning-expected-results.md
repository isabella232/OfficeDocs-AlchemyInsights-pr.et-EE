---
title: 1491-Search-Not-tagastamine-oodatud-tulemused
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740470"
---
# <a name="content-search-not-returning-expected-results"></a>Sisu otsing ei tagasta oodatud tulemeid

Microsoft 365 turbe & nõuetele vastavuse keskuses sisu otsimisel võidakse kuvada ootamatud otsingutulemused. Arvestage järgmiste asjadega, mis võivad teie otsingutulemusi mõjutada.

- **Sisu asukohad ja otsingukriteeriumid**: Veenduge, et olete valinud õige sisu asukohad ja otsingu tingimused. Kui käivitasite suure otsingu (paljudes asukohtades), kaaluge selle tükeldamist mitmeks otsinguks.

- **Osaliselt indekseeritud üksused**: postkastidest  [osaliselt indekseeritud üksused](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) kaasatakse hinnangulise otsingu tulemisse. Siiski ei kuulu SharePointi ja OneDrive ' i saitidelt osaliselt indekseeritud üksused otsingu hinnangusse.

- **Otsingu tõrked**: suurel hulgal postkastidest (üle 100 000 postkasti) otsimisel võite saada tõrketeateid, kus on tõrkekoodid (nt CS008-009 ja CS012-002). Sellisel juhul proovige otsingut ainult ebaõnnestunud sisu asukohtade korral. Lisateavet leiate  [sellest artiklist](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
