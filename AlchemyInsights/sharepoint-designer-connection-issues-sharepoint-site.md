---
title: SharePoint Designer connection issues
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942021"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer connection issues 

Kui SharePoint kujundajal on probleeme SharePoint saitidega, proovige järgmisi levinud lahendusi.

1. juhis: SharePoint Designer 2013 [värskendatakse SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [SharePoint Designer 2013 2.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)augusti värskendusega.



2. juhis. Tühjendage kohalikud vahemälufailid.

1. Sulgege SharePoint Designer 2013.

2. Eemaldage kohalikus arvutis kõik järgmistes kaustades olevad failid.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avage SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.

3. [juhis. Modernautentimise lubamine Office 2013 Windows seadmetes.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

4. juhis. Administraatorid peavad SharePoint administraatorikeskuse sätetes lubama SharePoint.  Lisateavet [leiate teemast Kohandatud skriptide lubamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) või keelamine.


