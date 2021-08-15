---
title: Diagnostika erinevate portide juurdepääsuprobleemide jaoks
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030898"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostika erinevate portide juurdepääsuprobleemide jaoks

Erinevate portide juurdepääsuprobleemide lahendamiseks tehke järgmist.

1. Peatage/jaotage virtuaalarvuti (VM) portaalist, taaskäivitage VM ja testige uuesti. 
2. Kontrollige oma VM-i võrgusätteid, et teha kindlaks, kas võrguturberühmad (NSGs) blokeerivad liiklust. Samuti saate [](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) võrguvahiku IP-voo kontrollimise tööriista abil kontrollida, kas NSG-d blokeerivad liiklust, User-Defined Marsruudid (UDR- id) suunavad teie liikluse tagasi kohapealse (vaikemarsruudi 0.0.0.0/0) või võrguseadmesse.
Kui teil esineb pärast ülaltoodud juhiste proovimist endiselt probleeme, sisestage vm-nimi ja TCP-port, mida proovite edasiseks diagnoosimiseks meili saata.

**Soovitatud dokumendid**

[Piirangud ja soovitused väljaminevate meilisõnumite saatmiseks üle pordi 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)