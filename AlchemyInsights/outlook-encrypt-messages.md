---
title: S/MIME Outlookis veebis
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752856"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-kirjade krüptimine Outlookis

Office 365 sõnumi krüptimine on loodud Microsoft Azure Rights Management (Azure RMS), mis on osa Azure ' i teabekaitse. Kui teie tellimus sisaldab Azure ' i õiguste haldust või Azure ' i Teabekaitset, ei ole õiguste halduse teenuse **käsitsi lubamiseks või aktiveerimiseks vaja toiminguid** teha.

Kliendi tagasiside põhjal ei saa me enam lubada Exchange ' i meilivoolu reegleid automaatselt krüptida Väljamineva meili, mis sisaldab teatud tüüpi tundlikku teavet teie rentnikus vaikimisi. Selle asemel pakume üksikasjalikke juhiseid selle kohta, kuidas te saate seda ise teha. Lisateabe saamiseks selle kohta, kuidas luua transpordireegel tundliku teabe krüptimiseks, lugege [seda artiklit](https://aka.ms/OmeEtr).

- Kui kasutate Outlook Web (endine **OWA**): koostamisel e-kirja, klõpsake lihtsalt **kaitsta** OWA. See kehtib "ära Edasta" luba. Klõpsake nuppu **Muuda luba** ja valige **Krüpti** ainult sõnumi krüptimiseks.

- Kui kasutate **Outlooki kliendi**: krüptitud sõnumi saatmiseks Outlook 2013 või 2016 või Outlook 2016 for Mac, valige **Suvandid** > **permissions**, seejärel valige kaitse valik, mida vajate.

- **Automaatselt krüptida kõik saadetud e-posti** teatud adressaatidele või väliste partnerite organisatsioonidele, peate looma voog transpordi reegel Exchange ' i halduskeskus. Üksikasjalikud juhised on antud [tugiteenuste artiklis](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

