---
title: Töövoomeili ei saadeta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072516"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Töövoomeili ei saadeta SharePoint või teegi jaoks

1. Töövoo meilisõnumeid ei saadeta kõigile kasutajatele ega ainult kindlatele kasutajatele või kuvatakse tõrketeade Meilisõnumit ei saa saata. Veenduge, et **meilisõnumil oleks sobiv adressaat.**

    Kontrollige, kas kasutaja on selle **saidikogumi** jaotises Kõik inimesed (kasutajateabe loend) olemas.  Otse-URL-i näidis: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Kui kasutajat pole olemas, veenduge, et kasutaja oleks lehele sisse logitud. 
    - Kui tegemist on välise kasutajaga, veenduge, et tema kutse oleks aktsepteeritud.
    - Kui kasutaja on õiguste rühmas olemas, veenduge, et meiliaadress oleks õige.
    - Kui kasutajate meiliaadressi pole siin määratud, looge selle kasutaja jaoks näidisteatis, mis sunnib selle kasutajakonto sünkroonima SharePoint selle saidikogumi kasutajaprofiilidega.
 
2. Töövood saadetakse saidikogumi administraatoritele, kuid mitte teistele kasutajatele, ja kuvatakse **tõrge HTTP Keelatud <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Lugege [teemat Juurdepääs keelatud, kui saadate meilisõnumi SharePoint rühma.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Samuti veenduge, et **piiratud juurdepääsuga kasutaja õiguste lukustusrežiimi** saidikogumi funktsioon pole aktiivne.


## <a name="related-topics"></a>Seotud teemad
Kas soovite proovida Microsoft Flow SharePoint Online'is?
- [Loo Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


