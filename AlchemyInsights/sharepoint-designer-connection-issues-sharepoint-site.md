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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716888"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer ühenduse probleemid 

<p>Kui SharePoint Designer on praegu ühenduse probleemid SharePointi saitidele, proovige järgmisi ühiseid lahendusi.</p> <p><strong>Samm 1:</strong> <strong>Kontrollida SharePoint Designeri uuendatakse&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Värskendus SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Samm 2:</strong> <strong>Tühjendage kohalik cache faile</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Sulgege SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Kohalikus arvutis sirvides eemaldama vahemällu salvestatud failid järgmisi kaustu.&nbsp;</li> <li style="font-weight: 400;">Klõpsake <strong>alustada -&gt; käivitada</strong> ja kustutage kõik failid leiate, kui iga selle alla asukohad.&nbsp;<br /><br />%AppData%\Microsoft\Web server Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Avada SharePoint Designer 2013 ja sisestage konto uuesti, et näha, kas see töötab.</li> </ol> <p><strong>Samm 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Windowsi seadmetes Office 2013 kaasaegne autentimise</strong></a>&nbsp;</p> <p><strong>Samm 4:</strong> <strong>Administraatorid peavad võimaldama kohandatud skripti SharePoint Designeri ühenduse lubamiseks</strong>.</p> <p>Leiate täpsed juhised, näidised ja arvestamine <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Luba või kohandatud skripti</a>.&nbsp;</p>


