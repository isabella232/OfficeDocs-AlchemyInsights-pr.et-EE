---
title: Jõudluse probleemid – SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771897"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePointi või OneDrive ' i aeglased, kättesaamatud või kättesaamatud mitme kasutaja jaoks

SharePointis või OneDrive ' is võivad olla aeglased, kättesaamatud või kättesaamatud või kuvada mitu põhjust teenust kättesaamatuks või 503 tõrkeks.
  
- Kui teie SharePointi või OneDrive ' i sait on mitme kasutaja jaoks aeglane või hilinenud, võib esineda ajutine teenus, kus kasutajad saavad SharePointi saitidele või OneDrive ' i sisule juurdepääsul kasutada ajutisi viivitusi või navigeerimine. Kontrollige [teenuse tervise armatuurlauda](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , et näha, kas teie ettevõte on mõjutatud.
  
- Kui proovite liikuda SharePointi või OneDrive ' i saitidele, võivad kasutajad saada *503 serveriga hõivatud* tõrke. Selle tõrke põhjuseks võib olla SharePointi teenuse ahendamine. SharePoint Online kasutab SharePoint Online’i teenuste optimaalse jõudluse ja töökindluse säilitamiseks ahendamist. Ahendamine piirab kasutajate toimingute või samaaegsete kõnede arvu (skripti või koodi poolt), et ennetada ressursside ülekasutamist. Lisateavet ahendamise kohta leiate artiklist [SharePoint Online ' is ahendamise või blokeerimise vältimine](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Kui teil ilmneb väike jõudlus **klassikalise** või **moodsa** SharePointi saidi või lehega, kasutage lehtede analüüsimiseks [lehte diagnostilist tööriista](https://aka.ms/perftool) .
  
- Kui teil on endiselt üldine aegluse, vaadake selle artikli allosas olevaid ressursse: [SharePoint Online ' i jõudluse häälestamise tutvustus](https://go.microsoft.com/fwlink/?linkid=2024334)
  