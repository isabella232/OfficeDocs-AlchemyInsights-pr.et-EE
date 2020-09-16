---
title: Jõudluse probleemid – SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771240"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePointi või OneDrive ' i aeglased, kättesaamatud või kättesaamatud mitme kasutaja jaoks

Kui OneDrive ' i või SharePointi sait pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib olla ajutine teenuse probleem. [Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).

**Kasutaja lisamine ja litsentsimine**

Veenduge, et [määrate kasutajatele Microsoft 365 ettevõtetele litsentsid](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Õiguse määramine**

Kui kasutajale on määratud SharePointi litsents ja ta saab endiselt juurdepääsu keelava sõnumi, siis veenduge, et neil on määratud [õigusetasemed](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Accessi taotluse funktsiooni kasutamine**

[Accessi taotluse funktsioon](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) võimaldab inimestel taotleda juurdepääsu sisule, mida neil praegu ei ole.

**Kohandatud skripti lubamine võib põhjustada juurdepääsu keelatud probleemidele**

On teatud stsenaariumid, mille korral saab *kohandatud skripti funktsiooni lubada* , kui juurdepääs on keelatud. Mõjutatud funktsioonide loendi, turvalisuse kaalutlused ja funktsiooni keelamise võimalus. Vaadake teemat [kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

