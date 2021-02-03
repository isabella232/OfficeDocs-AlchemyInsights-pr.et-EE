---
title: EWS-s ahendussätete muutmine
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075893"
---
# <a name="changing-ews-throttling-settings"></a>EWS-s ahendussätete muutmine

Käivitage meie automaattest, mis lubab teil migreerimise ajaks muuta EWS-i ahenduspoliitikat. Võtke arvesse, et isegi pärast selle käitamist kehtib EWS-i importimiste kohta endiselt piirang 150 MB 5 minuti ja ühe postkasti kohta; migreerimise läbilaskekiiruste suurendamiseks migreerige ühekorraga suurem arv kasutajaid.

Võtke arvesse, et EWS-i ahenduspoliitika muudatused ei mõjuta järgmisi migreerimistüüpe (milleks kasutatakse Microsofti tööriistu): hübriidne, ületõste/etapiviisiline (RPC/HTTP), IMAP, G Suite, avalik kaust või PST imporditeenus.