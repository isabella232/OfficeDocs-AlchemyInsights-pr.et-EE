---
title: Töövoo meilisõnumit ei saadeta
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748985"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>SharePointi loendi või teegi jaoks ei saadeta töövoo meilisõnumeid

1. Töövoote meilisõnumeid ei saadeta kõigile kasutajatele ega ainult kindlatele kasutajatele või kuvatakse tõrketeade, et **meilisõnumit ei saa saata. Veenduge, et meilisõnumil on sobiv adressaat**.

    Kontrollige, kas kasutaja on selle saidikogumi rühmas " **kõik inimesed** " permissions (kasutajateabe loend) olemas.  Proovi Direct URL: https:// <tenant> . SharePoint.com/sites/ <sitename> /_Layouts/15/People.aspx? MembershipGroupId = 0

    - Kui kasutajat pole olemas, veenduge, et kasutaja on lehele sisse logitud. 
    - Kui see on väline kasutaja, veenduge, et nende kutse on aktsepteeritud.
    - Kui kasutaja on rühmas permissions olemas, veenduge, et meiliaadress oleks õige.
    - Kui kasutajate meiliaadressi pole siin määratud, looge selle kasutaja jaoks hoiatusteade, mis sunnib selle kasutajakonto sünkroonima SharePointi kasutajaprofiilide kaudu selle saidikogumi jaoks.
 
2. Töövoogudest saadav meilisõnum saadetakse Saidikogumi administraatoritele, kuid mitte teistele kasutajatele ja HTTPS-i HTTPS-i **keelatud tõrketeate https <span>:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendEmail**.
 

    Vaadake teemat [juurdepääs on keelatud, kui saadate meilisõnumi SharePointi rühmale](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Samuti veenduge, et **piiratud juurdepääsuga kasutaja õiguste lukustamise režiimi** saidikogumi funktsioon pole aktiivne.


## <a name="related-topics"></a>Seotud teemad
Kas soovite proovida Microsoft Flow SharePoint Online ' is?
- [Voo loomine](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja voog](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


