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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968373"
---
# <a name="changing-ews-throttling-settings"></a>EWS-i ahendussätete muutmine

Käivitage meie automaattest, mis lubab teil migreerimise ajaks muuta EWS-i ahenduspoliitikat. Võtke arvesse, et isegi pärast selle käitamist kehtib EWS-i importimiste kohta endiselt piirang 150 MB 5 minuti ja ühe postkasti kohta; migreerimise läbilaskekiiruste suurendamiseks migreerige ühekorraga suurem arv kasutajaid.

Võtke arvesse, et EWS-i ahenduspoliitika muudatused ei mõjuta järgmisi migreerimistüüpe (milleks kasutatakse Microsofti tööriistu): hübriidne, ületõste/etapiviisiline (RPC/HTTP), IMAP, G Suite, avalik kaust või PST imporditeenus.