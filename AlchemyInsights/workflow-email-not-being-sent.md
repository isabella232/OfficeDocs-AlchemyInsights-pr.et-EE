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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530865"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>SharePointi loendi või teegi ei saadetakse töövoo e-posti

1. Töövoogude meilisõnumeid ei saadeta kõik kasutajad või ainult teatud kasutajatele või näete viga **e-kirja ei saa saata. Veenduge, et meilisõnumil sobiv adressaat**.

    Kontrollige, kas kasutajal on olemas **Kõigi inimeste** õiguste rühma (kasutaja info loendi) selle saidikogumi.  Proovi otse URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Kui kasutaja olemas, veenduge, et kasutaja on sisse logitud lehe. 
    - Kui on välise kasutaja, veenduge, et nende kutse on aktsepteeritud.
    - Kui kasutaja õiguste rühma, veenduge, et meiliaadress on õige.
    - Kui kasutajate e-posti aadress ei ole siin seatud, looge selle kasutaja, mis sunnib selle kasutaja konto sünkroonimine SharePointi kasutaja profiilid selles saidikogumis näidisteate.
 
2. Töövoogude meilisõnumeid saadetakse saidi administraatorid, kuid mitte teistele kasutajatele ja kuvada tõrge **HTTP Forbidden et <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Vaata [Juurdepääs keelatud, SharePointi rühmale e-kirja saatmisel](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Samuti veenduge, et **piiratud juurdepääsuga kasutaja luba lockdown režiim** saidi kogumise funktsioon pole aktiivne.


## <a name="related-topics"></a>Seotud teemad
Tahan proovida Microsoft Flow SharePoint Online?
- [Luua voolu](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja voolu](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


