---
title: SharePoint Designer ühenduse probleemid
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508419"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer ühenduse probleemid 

Kui SharePoint Designer on praegu ühenduse probleemid SharePointi saitidele, proovige järgmisi ühiseid lahendusi.

1. samm: Veenduge, et SharePoint Designer 2013 on uuendanud [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ja [2 August 2016 värskendus SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. samm: Kustutage kohalik cache faile:

1. Sulgege SharePoint Designer 2013.

2. Kohalikus arvutis eemaldada igas järgmistest kaustadest kõik failid.

    - %AppData%\Microsoft\Web server Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Avada SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.

3. samm: [Windowsi seadmetes Office 2013 kaasaegne autentimise](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

4. samm: Administraatorid tuleb **Lubada kohandatud skripti** seaded SharePointi administreerimiskeskuse SharePoint Designeri ühenduse lubamiseks. Vt [Luba või kohandatud skripti](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) lisateabe saamiseks.


