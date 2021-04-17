---
title: Meilisõnumite püüdmise loomine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816196"
---
# <a name="create-an-email-catch-all"></a>Meilisõnumite püüdmise loomine

Saagi kasutamist ei soovitata. Parem on pakkuda saatjale tagasisaatmine, andes saatjale teada, et tema sõnumit ei saanud adressaadina kohale toimetada, et nad saaksid midagi ette võtta. Samuti saate jälgitud postkasti piirata ainult varem kehtivate meiliaadresside püüdmisega. 

Iga postkast saab palju rämpsposti ja võib lõpuks täita, kui seda ei jälgita hoolikalt. (Piirangud on olemas.) 

Kui otsustate jätkata, tehke järgmist.

1. Dünaamilise levirühma loomine & "Kõik adressaaditüübid".

2. Looge spetsiaalne postkast meilisõnumite püüdmiseks , näiteks catchall@domain.com.

3. Määrake konkreetse domeeni domeenitüübiks "InternalRelay". Kui eemaldate hiljem kogu saagi, määrake domeen kindlasti uuesti autoriteetseks.

4. Looge meilivoo transpordireegel järgmiselt.

    - Kui saatja on "Väljaspool asutust"
    - Sõnumi ümbersuunamine Catchall@domain.com
    - Välja arvatud juhul, kui adressaat on allusers@domain.com liige (levirühm sisaldab kõiki liikmeid)
    - Kontrollige, kas dünaamilise levirühma lisatakse uusi postkaste.
