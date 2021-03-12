---
title: Linuxi seadmes MDATP erandite konfigureerimine ja valideerimine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746019"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="7f135-102">Linuxi seadmes MDATP erandite konfigureerimine ja valideerimine</span><span class="sxs-lookup"><span data-stu-id="7f135-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="7f135-103">Saate välistada teatud failid, kaustad, protsessid ja protsessis avatud failid MDATP skannimise kaudu.</span><span class="sxs-lookup"><span data-stu-id="7f135-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="7f135-104">Välistused aitavad vältida tarkvara ja failide vale tuvastamist, mis on teie asutuse jaoks kordumatu või kohandatud.</span><span class="sxs-lookup"><span data-stu-id="7f135-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="7f135-105">Erandid aitavad leevendada ka MDATP põhjustatud jõudluse probleeme.</span><span class="sxs-lookup"><span data-stu-id="7f135-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="7f135-106">Lisateavet leiate teemast [MDATP jaoks mõeldud erandite konfigureerimine ja valideerimine](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="7f135-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7f135-107">Selles artiklis kirjeldatud erandid ei kehti muude MDATP jaoks, sh lõpp-punkti tuvastamine ja reageerimine (EDR).</span><span class="sxs-lookup"><span data-stu-id="7f135-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="7f135-108">Selles artiklis kirjeldatud meetodite abil välistavad failid võivad endiselt esile kutsuda ka EDR ning muid tuvastuse võimalusi.</span><span class="sxs-lookup"><span data-stu-id="7f135-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
