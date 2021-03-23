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
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="45a3a-102">Erinevate sadamate Accessi probleemide diagnostika</span><span class="sxs-lookup"><span data-stu-id="45a3a-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="45a3a-103">Erinevate pordi juurdepääsu probleemide lahendamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="45a3a-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="45a3a-104">Peatage/eraldage virtuaalarvuti (VM) portaalist, taaskäivitage VM ja testige uuesti.</span><span class="sxs-lookup"><span data-stu-id="45a3a-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="45a3a-105">Kontrollige oma VM-i võrgusätteid, et kindlaks teha, kas teil on võrgu turvalisuse rühmad (NSGs) liikluse blokeerimine.</span><span class="sxs-lookup"><span data-stu-id="45a3a-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="45a3a-106">Saate kasutada ka [Network watcheri IP-voo kinnitamise tööriista](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , et kontrollida NSGs, User-Defined marsruute (UDRs), marsruudid liiklust tagasi kohapealsesse ("vaikeprotsessi" 0.0.0.0/0) või võrguseadmesse.</span><span class="sxs-lookup"><span data-stu-id="45a3a-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="45a3a-107">Kui teil ilmneb pärast ülaltoodud juhiste järgimist endiselt probleeme, esitage VM-i nimi ja TCP-port, mida proovite saata meiliga edasiseks diagnoosimiseks.</span><span class="sxs-lookup"><span data-stu-id="45a3a-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="45a3a-108">**Soovitatud dokumendid**</span><span class="sxs-lookup"><span data-stu-id="45a3a-108">**Recommended Documents**</span></span>

[<span data-ttu-id="45a3a-109">Piirangud ja soovitused Väljamineva meili saatmiseks porti 25 kaudu</span><span class="sxs-lookup"><span data-stu-id="45a3a-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)