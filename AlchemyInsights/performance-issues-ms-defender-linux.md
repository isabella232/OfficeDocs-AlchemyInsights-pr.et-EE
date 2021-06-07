---
title: Microsoft Defender for Endpointi jõudlusprobleemid Linuxis
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793759"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="26524-102">Microsoft Defender for Endpointi jõudlusprobleemid Linuxis</span><span class="sxs-lookup"><span data-stu-id="26524-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="26524-103">Selles artiklis juhendatakse teid Microsoft Defender for Endpointi jõudlusprobleemide tuvastamise juhistest Linuxis.</span><span class="sxs-lookup"><span data-stu-id="26524-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="26524-104">Oluline on esmalt veenduda, et teie probleem on lahendatud uusima [versiooniga.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="26524-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="26524-105">Uurimise alustamiseks lugege teemat Microsoft [Defender for Endpointi jõudlusprobleemide tõrkeotsing Linuxis.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="26524-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="26524-106">Välistamised</span><span class="sxs-lookup"><span data-stu-id="26524-106">Exclusions</span></span>

<span data-ttu-id="26524-107">Välistamised võivad aidata jõudlusprobleeme leevendada.</span><span class="sxs-lookup"><span data-stu-id="26524-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="26524-108">Vaadake oma välistamised üle enne alustamist, et mis tahes täiendav risk oleks teada ja dokumenteeritud.</span><span class="sxs-lookup"><span data-stu-id="26524-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="26524-109">Lisateavet leiate teemast Microsoft Defenderi välistamiste konfigureerimine ja [valideerimine Lõpp-punkti jaoks Linuxis.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="26524-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="26524-110">Kui teil on mitu & kausta, mille soovite välistada ja need on kõik samas ühenduspunktis, võib ühenduspunkti välistamine olla lihtsam.</span><span class="sxs-lookup"><span data-stu-id="26524-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="26524-111">Alates veebruari väljaandest 101.22.80 saate välistada kogu ühenduspunkti.</span><span class="sxs-lookup"><span data-stu-id="26524-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="26524-112">Näiteks kui /mnt/backup on mountpoint, saate välistamisloendisse lisada /mnt/backup, käivitades selle käsu.</span><span class="sxs-lookup"><span data-stu-id="26524-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="26524-113">**Märkus.** Välistamiste lisamine suurendab ründevara tuvastamata jätmise ohtu ning seda tuleks käsitleda ja rakendada hoolikalt.</span><span class="sxs-lookup"><span data-stu-id="26524-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="26524-114">Kas vajate abi?</span><span class="sxs-lookup"><span data-stu-id="26524-114">Need Help?</span></span>

<span data-ttu-id="26524-115">Selleks et teid kõige tõhusamal viisil aidata, koguge diagnostikaandmed enne tugiteenuse juhtumi avamist.</span><span class="sxs-lookup"><span data-stu-id="26524-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
