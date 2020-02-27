---
title: Loo e-posti saagi kõik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286106"
---
# <a name="create-an-email-catch-all"></a>Loo e-posti saagi kõik

Saagi kasutamine on tugevalt heidutatud. Parem on anda tagasilöök saatjale, kes laseb saatjatel teada, et nende sõnumit ei saanud saata nii, et nad saaksid tegutseda. Samuti saate piirata jälgida postkasti ainult püüda varem kehtiv e-posti aadressid. 

Iga saagi kõik postkast saab palju rämpsposti ja võib lõpuks täita, kui ei ole tähelepanelikult jälgida. (On olemas piirangud.) 

Kui otsustate jätkata, toimige järgmiselt.

1. Dünaamilise levirühma & loomiseks lisage "kõik adressaadi tüübid".

2. Looge spetsiaalne postkast püüda e-kirju, näiteks catchall@domain.com.

3. Konkreetse domeeni, seadke DomainType "Internalrelee". Kui te hiljem eemaldada saagi kõik, kindlasti seadke domeeni tagasi autoriteetne.

4. Loo Mailflow transport reegel järgmiselt:

    - Kui saatja on "väljaspool organisatsiooni"
    - Suuna sõnum Catchall@domain.com
    - Välja arvatud juhul, kui adressaat on allusers@domain.com liige (levirühm sisaldab kõiki liikmeid)
    - Veenduge, et uus postkastid lisatakse dünaamiline jaotus rühma kinnitada
