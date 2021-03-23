---
title: Erinevate sadamate Accessi probleemide diagnostika
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035262"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Erinevate sadamate Accessi probleemide diagnostika

Erinevate pordi juurdepääsu probleemide lahendamiseks tehke järgmist.

1. Peatage/eraldage virtuaalarvuti (VM) portaalist, taaskäivitage VM ja testige uuesti. 
2. Kontrollige oma VM-i võrgusätteid, et kindlaks teha, kas teil on võrgu turvalisuse rühmad (NSGs) liikluse blokeerimine. Saate kasutada ka [Network watcheri IP-voo kinnitamise tööriista](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , et kontrollida NSGs, User-Defined marsruute (UDRs), marsruudid liiklust tagasi kohapealsesse ("vaikeprotsessi" 0.0.0.0/0) või võrguseadmesse.
Kui teil ilmneb pärast ülaltoodud juhiste järgimist endiselt probleeme, esitage VM-i nimi ja TCP-port, mida proovite saata meiliga edasiseks diagnoosimiseks.

**Soovitatud dokumendid**

[Piirangud ja soovitused Väljamineva meili saatmiseks porti 25 kaudu](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)