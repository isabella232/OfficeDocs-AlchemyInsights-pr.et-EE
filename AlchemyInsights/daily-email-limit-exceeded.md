---
title: Igapäevase e-posti piirmäär on ületatud. Töövoog on peatatud.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514444"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Igapäevase e-posti on ületatud. Töövoog on peatatud.

See tõrge võib vastu võtta järgmistel juhtudel:

- Olete töövoo SharePoint Online, mis kasutab SharePoint 2010 või SharePointi 2013 töövoo platvormi tüüp.
- Töövoog on konfigureeritud kohandatud e-kirja saatmiseks üle 200 kasutajatele korraga, üle 10 000 adressaati päevas või üle 30 sõnumites minutis.
- Töövoo käivitamisel saadetakse e-kiri ja märkate järgmist käitumist:
    - Kasutades SharePointi 2013 platvormi tüüp töövoo sirvite **Töövoo oleku** lehel. Lehe Töövoo olek **Staatusest** on seatud **Alustatud**ja teabe õhupalli kuvab **ei saa adressaadile saata**.

Selle probleemi lahendamiseks konfigureerige oma töövoo saata e-kirju [Exchange Online'i saatja piire](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)ületamata. Näiteks kasutada töövoo pausi, saada email Office 365 rühma, leviloendi või e-posti lubatud turberühma või saata sõnum alla 200 adressaadile korraga.


Lisateabe saamiseks vaadake [artikli](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Seotud teemad
- [Luua voolu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja voolu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 