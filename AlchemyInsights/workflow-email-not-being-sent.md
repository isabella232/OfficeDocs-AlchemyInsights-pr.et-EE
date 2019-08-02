---
title: Töövoo e-posti ei ole saadetud
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
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059600"
---
# <a name="workflow-email-is-not-being-sent"></a>Töövoo e-posti ei ole saadetud

1. Töövoogude meilisõnumeid ei saadeta kõik kasutajad või ainult teatud kasutajatele või näete viga **e-kirja ei saa saata. Veenduge, et meilisõnumil sobiv adressaat**.

Kontrollige, kas kasutajal on olemas **Kõigi inimeste** õiguste rühma (kasutaja info loendi) selle saidikogumi.  Proovi otse URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

- Kui kasutaja olemas, veenduge, et kasutaja on sisse logitud lehe. 
- Kui on välise kasutaja, veenduge, et nende kutse on aktsepteeritud.
- Kui kasutaja õiguste rühma, veenduge, et meiliaadress on õige.
- Kui kasutajate e-posti aadress ei ole siin seatud, looge selle kasutaja, mis sunnib selle kasutaja konto sünkroonimine SharePointi kasutaja profiilid selles saidikogumis näidisteate.
 
2. Töövoogude meilisõnumeid saadetakse saidi administraatorid, kuid mitte teistele kasutajatele ja kuvada tõrge **Forbidden HTTP- <spam> <spam> ** <spam> <spam>.
 

Vaata [Juurdepääs keelatud, kui saadetud e-pakuvad](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

Samuti veenduge, et **piiratud juurdepääsuga kasutaja luba lockdown režiim** saidi kogumise funktsioon pole aktiivne.

## <a name="related-topics"></a>Seotud teemad
- [Luua voolu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja voolu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


