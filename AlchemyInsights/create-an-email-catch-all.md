---
title: Kõigi meilisõnumite loomine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712982"
---
# <a name="create-an-email-catch-all"></a>Kõigi meilisõnumite loomine

Saagi kasutamine on tugevalt heidutav. Parem on anda põrge tagasi saatjale, et saatjad saaksid teada, et nende sõnumit ei saanud esitada nii, et nad saaksid tegutseda. Samuti saate jälgida postkasti piirata ainult varem kehtivate meiliaadresside järgi. 

Kõik postkastid saavad palju rämpsposti ja võivad lõpuks täita, kui neid hoolikalt ei jälgita. (Seal saab limiite.) 

Kui otsustate jätkata, järgige järgmisi juhiseid.

1. Saate luua dünaamilise levirühma & kaasata "kõik adressaadi tüübid".

2. Saate luua spetsiaalse postkasti meilisõnumite püüdmiseks (nt catchall@domain.com).

3. Määrake konkreetse domeeni jaoks DomainType väärtuseks "InternalRelay". Kui eemaldate selle hiljem, veenduge, et Domeen oleks uuesti autoriteetseks määratud.

4. Meilivoogude transpordi reegli loomiseks tehke järgmist.

    - Kui saatja on "väljaspool asutust"
    - Sõnumi ümbersuunamine Catchall@domain.com
    - Välja arvatud juhul, kui adressaat on allusers@domain.com liige (levirühma sisaldab kõiki liikmeid)
    - Veenduge, et valideerite, et uued postkastid lisatakse dünaamilisse levirühma.
