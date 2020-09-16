---
title: SharePoint Designeri ühenduste probleemid
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727167"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designeri ühenduste probleemid 

Kui SharePoint Designeris esineb SharePointi saitidel probleeme, proovige järgmisi levinud lahendusi.

1. juhis: Veenduge, et SharePoint Designer 2013 oleks värskendatud SharePoint Designeri [hoolduspaketiga Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja sharepoint [Designer 2013, August 2, 2016 värskendus](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. juhis: tühjendage kohaliku vahemälu failid.

1. Sulgege SharePoint Designer 2013.

2. Eemaldage kohalikus arvutis kõik järgmistest kaustadest leitud failid.

    - %APPDATA%\Microsoft\Web serveri Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avage SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.

3. juhis: [Windowsi seadmetes Office 2013 kaasaegse autentimise lubamine](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4. juhis: Administraatorid peavad **lubama kohandatud skripti** SharePointi administreerimiskeskuse sätetes, et lubada SharePoint Designeri ühendust. Lisateavet leiate teemast [kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


