---
title: Päevane meililimiit on ületatud. Töövoog on peatatud.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914647"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päevane meililimiit on ületatud. Töövoog on peatatud.

See tõrge võidakse kuvada järgmistel juhtudel.

- Teil on SharePoint Online'is töövoog, mis kasutab SharePoint 2010 või SharePoint 2013 töövooplatvormi tüüpi.
- Töövoog on konfigureeritud saatma kohandatud meilisõnumi korraga rohkem kui 200 kasutajale, üle 10 000 adressaadi päevas või rohkem kui 30 sõnumit minutis.
- Töövoo käivitamisel meilisõnumit ei saadeta ja märkate järgmist käitumist.
    - Töövoo korral, mis kasutab SharePoint 2013 platvormitüüpi, sirvige lehele **Töövoo olek.** Lehel Töövoo olek on ettevõttesisene **olek** seatud väärtusele **Alustatud** ja teabemull kuvab **väärtuse Ei saa adressaadile saata.**

Selle probleemi lahendamiseks konfigureerige töövoog meilisõnumite saatmiseks, ületamata [Exchange Online piiranguid.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) Näiteks saate töövoos pausi teha, saata meilisõnumi Microsoft 365 rühmale, levirühmale või meiliga lubatud turberühmale või saata sõnumi korraga vähem kui 200 adressaadile.


Lisateavet leiate järgmisest [artiklist.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Seotud teemad
- [Loo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 