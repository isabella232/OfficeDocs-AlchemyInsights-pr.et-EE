---
title: Päevane e-posti limiit on ületatud. Töövoog on peatatud.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731559"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Päevane e-posti limiit on ületatud. Töövoog on peatatud.

Selle tõrke võib vastu võtta järgmistel juhtudel.

- Teil on SharePoint Online ' is töövoog, mis kasutab SharePoint 2010 või SharePoint 2013 töövoo platvormi tüüpi.
- Töövoog on konfigureeritud saatma kohandatud meilisõnumeid rohkem kui 200 kasutajale korraga, üle 10 000 adressaadi päevas või rohkem kui 30 sõnumit minutis.
- Töövoo käivitamisel meilisõnumit ei saadeta ja te märkate järgmist käitumist.
    - SharePointi 2013 platvormi tüübiga töövoo korral sirvige lehe **töövoo olek** kaudu. Töövoo oleku lehel on **sisemine olekuks** seatud **Alustatud**ja teabe jutumull **ei saa adressaadile saata**.

Selle probleemi lahendamiseks konfigureerige oma töövoog meilisõnumite saatmiseks, ületamata seejuures [Exchange Online ' i saatja limiite](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Näiteks saate töövoos kasutada pausi, saata meilisõnumi Microsoft 365 rühmale, levirühma või e-posti loaga turberühma või saata sõnumi korraga vähem kui 200 adressaadile.


Lisateavet leiate järgmisest [artiklist](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Seotud teemad
- [Voo loomine](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja voog](https://flow.microsoft.com/blog/sharepoint-and-flow/) 