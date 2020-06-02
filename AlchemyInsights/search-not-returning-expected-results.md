---
title: 1491-otsing-mitte-tagasi oodatud-tulemused
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510568"
---
# <a name="content-search-not-returning-expected-results"></a>Sisu otsing ei tagasta oodatud tulemusi

Microsoft 365 Security & vastavuse Center sisu otsingud käivitamisel võidakse kuvada ootamatuid otsingutulemeid. Kaaluge järgmisi toiminguid, mis võivad teie otsingutulemeid mõjutada:

- **Sisu asukohad ja otsingutingimused**: Veenduge, et olete valinud õiged sisu asukohad ja otsingutingimused. Kui te käivitasite suure otsingu (paljude asukohtadest), kaaluge selle tükeldamist mitmesse otsingusse.

- **Osaliselt indekseeritud üksused**: postkastidest [osaliselt indekseeritud üksused](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) kaasatakse hinnangulisest otsingutulemustest. Kuid osaliselt indekseeritud üksused SharePoint ja OneDrive saidid ei sisaldu otsingu hinnang.

- **Otsingu tõrked**: otsides suur hulk postkastid (üle 100 000 postkastid), võite saada otsingu tõrked, TÕRKEKOODIDEST nagu CS008-009 ja CS012-002). Sel juhul proovige otsingut ainult nurjunud sisu asukohtade puhul. Vaadake [seda artiklit](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) lisateabe saamiseks.
