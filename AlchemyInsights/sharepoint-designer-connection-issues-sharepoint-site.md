---
title: SharePoint Online'i õiguste tasemed
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760689"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer ühenduse probleemid 

Kui SharePoint Designer on praegu ühenduse probleemid SharePointi saitidele, proovige järgmisi ühiseid lahendusi.

1. samm: Kontrollige SharePoint Designeri uuendatakse.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Värskendus SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

2. samm: Kustutage kohalik cache faile

- Sulgege SharePoint Designer 2013.

- Kohalikus arvutis sirvides eemaldama vahemällu salvestatud failid järgmisi kaustu.

- Klõpsake nuppu Start, Run ja Kustuta kõik failid leiate iga selle alla asukohad.

%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Avada SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.

3. samm: [Windowsi seadmetes Office 2013 kaasaegne autentimise](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

4. samm: Pead administraatorid lubada kohandatud skripti SharePoint Designeri ühenduse lubamiseks.

Leiate täpsed juhised, näidised ja arvestamine [Luba või kohandatud skripti](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


