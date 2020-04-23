---
title: Töövoo e-posti ei saadeta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766129"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Töövoo e-posti ei saadeta SharePointi loendi või teegi

1. Töövoogude e-posti ei saadeta kõigile kasutajatele või ainult teatud kasutajatele või kuvatakse tõrge **meilisõnumit ei saa saata. Veenduge, et meilisõnumil oleks kehtiv adressaat**.

    Kontrollige, kas kasutaja on olemas selle saidikogumi **kõik inimesed** õigused rühma (kasutaja teabe loend).  Näidis Direct URL: https://<tenant>. sharepoint.com/sites/<sitename>/_Layouts/15/People.aspx? MembershipGroupId = 0

    - Kui kasutajat pole olemas, veenduge, et kasutaja on lehele sisse logitud. 
    - Kui see on väline kasutaja, veenduge, et nende kutse on aktsepteeritud.
    - Kui kasutaja on olemas õiguste rühma, veenduge, et e-posti aadress on õige.
    - Kui kasutaja e-posti aadress on seatud siin, siis luua selle kasutaja näidisteatis, mis sunnib selle kasutajakonto sünkroonimine SharePointi kasutajaprofiilid selle saidikogumi.
 
2. E-posti töövoogude saadetakse saidikogumi administraatorid, kuid mitte teiste kasutajate ja **http keelatud <span>https</span>-i tõrge://URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendEmail**.
 

    Vaadake [juurdepääs keelatud, kui saadate e-kirja SharePointi rühma](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Samuti veenduge, et **piiratud juurdepääsuga kasutaja õiguste Lockdown režiimi** saidikogumi funktsioon ei ole aktiivne.


## <a name="related-topics"></a>Seotud teemad
Soovite proovida Microsoft Flow SharePoint Online?
- [Voo loomine](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePointi ja voog](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


