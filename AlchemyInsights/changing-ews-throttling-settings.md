---
title: EWS-i ahendussätete muutmine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818032"
---
# <a name="changing-ews-throttling-settings"></a>EWS-i ahendussätete muutmine

Käivitage meie automaattest, mis lubab teil migreerimise ajaks muuta EWS-i ahenduspoliitikat. Võtke arvesse, et isegi pärast selle käitamist kehtib EWS-i importimiste kohta endiselt piirang 150 MB 5 minuti ja ühe postkasti kohta; migreerimise läbilaskekiiruste suurendamiseks migreerige ühekorraga suurem arv kasutajaid.

Võtke arvesse, et EWS-i ahenduspoliitika muudatused ei mõjuta järgmisi migreerimistüüpe (milleks kasutatakse Microsofti tööriistu): hübriidne, ületõste/etapiviisiline (RPC/HTTP), IMAP, G Suite, avalik kaust või PST imporditeenus.