---
title: 2609-säilitamine-või-eDiscovery-hoidke
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994058"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Ei saa kustutada üksusi SharePoint Online ' i või OneDrive for Business

Teie või teie kasutajad ei saa kustutada SharePoint Online ' i või OneDrive for Business üksusi, kuna säilituspoliitika, säilitamise silt või eDiscovery hoida SharePointi OneDrive saidi või mõne kindla üksuse. See hõlmab dokumendi, dokumendi versiooni, kausta, dokumenditeegi, loendi, rakenduse, saidi või saidikogumi kustutamist. Siin on mõned näited tõrketeadetest, mida võite saada, kui püüate kustutada üksust, mida säilitatakse:

- "Seda saiti ei saa kustutada, kuna see sisaldub eDiscovery Hold-või säilituspoliitikas."
- "See sait on vastavuse poliitika seatud blokeerida kustutamine"
- "Vastavuspoliitika blokeerib praegu selle saidi kustutamise"
- "See saidikogum ei saa kustutada, kuna see sisaldab saite, mis sisalduvad eDiscovery Hold-või säilituspoliitika"
- "Peate kustutama kõik üksused selles kaustas enne kausta kustutamist"
- "Selle üksuse versioone ei saa kustutada, kuna see on kinni-või säilituspoliitika"
- "Üksust ei saa kustutada, kui hoida"
- "Sellele üksusele rakendatud silt takistab selle redigeerimist või kustutamist"
- "Loend ei saa kustutada, kui hoidke või säilituspoliitika"
- "Loendit ei saa kustutada, kui see on blokeeritud või säilituspoliitika on rakendatud"

Üksuste kustutamiseks ühes neist stsenaariumidest tuleb eemaldada säilituspoliitika, säilitussilt või eDiscovery Hold (või sait tuleb säilituspoliitikast välja jätta). Peate kas keelata või välistada vastava Hold, mis põhjustab probleemi. Pärast säilituspoliitika või hoidke eemaldamist, võib kuluda kuni 24 tundi muudatuse jõustumiseks. 

Lisateabe saamiseks erinevate säilitamise ja hoidke funktsioone, mida saab rakendada SharePointi saidid ja OneDrive kontod, vaadake ühte järgmistest teemadest.

- [Säilituspoliitika ülevaade](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Säilitussiltide ülevaade](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Halda hoiab Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery hoiab](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Pärand saidi sulgemine ja kustutamise poliitikad](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
