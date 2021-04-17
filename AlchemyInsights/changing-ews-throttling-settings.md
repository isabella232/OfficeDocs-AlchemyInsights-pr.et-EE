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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="276c7-102">EWS-i ahendussätete muutmine</span><span class="sxs-lookup"><span data-stu-id="276c7-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="276c7-103">Käivitage meie automaattest, mis lubab teil migreerimise ajaks muuta EWS-i ahenduspoliitikat.</span><span class="sxs-lookup"><span data-stu-id="276c7-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="276c7-104">Võtke arvesse, et isegi pärast selle käitamist kehtib EWS-i importimiste kohta endiselt piirang 150 MB 5 minuti ja ühe postkasti kohta; migreerimise läbilaskekiiruste suurendamiseks migreerige ühekorraga suurem arv kasutajaid.</span><span class="sxs-lookup"><span data-stu-id="276c7-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="276c7-105">Võtke arvesse, et EWS-i ahenduspoliitika muudatused ei mõjuta järgmisi migreerimistüüpe (milleks kasutatakse Microsofti tööriistu): hübriidne, ületõste/etapiviisiline (RPC/HTTP), IMAP, G Suite, avalik kaust või PST imporditeenus.</span><span class="sxs-lookup"><span data-stu-id="276c7-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>