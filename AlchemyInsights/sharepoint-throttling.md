---
title: SharePoint Online ' i ahendamine
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931438"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online ' i ahendamine

**Oluline**: paljud SharePoint Online ' i ja OneDrive kliendid käivitada Business kriitilised rakendused teenuse, mis töötavad taustal. Nende hulka kuuluvad sisu migratsioon, andmete kadu vältimine (DLP) ja backup lahendused. Nendel enneolematul ajal me võtame meetmeid, et tagada SharePoint Online ' i ja OneDrive teenused on väga kättesaadav ja usaldusväärne oma kasutajatele, kes sõltuvad teenuse rohkem kui kunagi varem kaugtöö stsenaariume.

Selle eesmärgi toetuseks oleme rakendanud ranget ahendamise piiranguid taustal olevatele rakendustele (migratsioon, DLP ja backup lahendused) tööpäeval päeva jooksul. Te peaksite ootama, et need rakendused saavutavad nende aegade jooksul väga piiratud läbilaskevõime. Aga, õhtuti ja nädalavahetusel tundi piirkonna, teenus on valmis töötlema oluliselt suurem hulk taotlusi taustal apps.

**SharePoint Online ' i ahendamine**

SharePoint Online ' i kasutab ahendamine optimaalse jõudluse ja töökindluse SharePoint Online Service. Ahendamine piirab kasutajate toimingute või samaaegsete kõnede (skripti või koodi) arvu, et vältida ressursside ülekasutamist. Lisateabe saamiseks külastage allolevaid linke.

- [Vältige ahendamist või blokeeritud SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [Andmete migratsioon ja SPO ahendamine](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [SharePoint Online ja OneDrive ' i migreerimise kiirus](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [SharePoint Online ' i ahendamise käsitsemiseks, kasutades eksponentsiaalselt tagasi välja](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [Võimsuse planeerimine ja koormuse testimine SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

