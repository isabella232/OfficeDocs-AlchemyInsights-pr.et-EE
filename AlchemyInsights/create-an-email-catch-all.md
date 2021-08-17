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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080742"
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
