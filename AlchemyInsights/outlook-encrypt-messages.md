---
title: S/MIME Outlooki veebirakenduses
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772258"
---
# <a name="encrypt-email-messages-in-outlook"></a>Meilisõnumite krüptimine Outlookis

Microsoft 365 Sõnumite krüptimine on loodud Microsoft Azure ' i õiguste halduses (Azure RMS), mis on osa Azure ' i teabe kaitsest. Kui teie tellimus sisaldab Azure ' i õiguste haldus-või Azure ' i teabe kaitset, **ei pea te õiguste halduse teenuse käsitsi lubamiseks või aktiveerimiseks mingeid toiminguid** tegema.

Klientide tagasiside põhjal ei luba me enam Exchange ' i meilivoo reegleid automaatselt krüptida väljaminevaid meilisõnumeid, mis sisaldavad teatud tüüpi delikaatseid andmeid rentniku jaoks vaikimisi. Selle asemel pakume üksikasjalikke juhiseid selle kohta, kuidas saate seda ise teha. Lisateabe saamiseks selle kohta, kuidas luua tundliku teabe krüptimiseks transpordi reeglit, lugege [seda artiklit](https://aka.ms/OmeEtr).

- Kui kasutate Outlooki veebirakenduses (varem **OWA**): meilisõnumi koostamisel klõpsake lihtsalt nuppu **kaitse** OWA-s. See kehtib "Ära saada edasi" luba. Klõpsake nuppu **Muuda õigusi** ja valige ainult sõnumi krüptimiseks **Krüpti** .

- Kui kasutate **Outlooki klientrakendust**: krüptitud sõnumi saatmiseks rakendusest Outlook 2013 või 2016 või Outlook 2016 for Mac, valige **Suvandid**  >  **ja**seejärel valige soovitud kaitse suvand.

- Teatud adressaatidele või väliste partnerite organisatsioonidele saadetavate **meilisõnumite automaatseks krüptimiseks** peate Exchange ' i administreerimiskeskuses looma meilivoo transpordi reegli. [Selles tugiteenuse artiklis](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)on toodud üksikasjalikud juhised.

