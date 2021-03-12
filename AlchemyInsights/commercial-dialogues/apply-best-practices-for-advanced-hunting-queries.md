---
title: Täpsemate jahipidamise päringute heade tavade rakendamine
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746186"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="b2390-102">Täpsemate jahipidamise päringute heade tavade rakendamine</span><span class="sxs-lookup"><span data-stu-id="b2390-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="b2390-103">Tulemuste kiiremaks ja ajalõpute vältimiseks keerukate päringute käitamise ajal rakendage järgmisi häid tavasid.</span><span class="sxs-lookup"><span data-stu-id="b2390-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="b2390-104">Kui proovite uusi päringuid, kasutage alati limiiti, et vältida väga suurte tulemite tekkimist.</span><span class="sxs-lookup"><span data-stu-id="b2390-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="b2390-105">Samuti saate `count` määrata tulemikomplekti suuruse esialgse hinnangu.</span><span class="sxs-lookup"><span data-stu-id="b2390-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="b2390-106">Kasutage kõigepealt ajafiltreid.</span><span class="sxs-lookup"><span data-stu-id="b2390-106">Use time filters first.</span></span> <span data-ttu-id="b2390-107">Ideaaljuhul Piirake päringuid seitsme päevaga.</span><span class="sxs-lookup"><span data-stu-id="b2390-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="b2390-108">Lisage päringu alguses kohe pärast filtrit soovitud filtrid, et enamik andmeid eemaldada.</span><span class="sxs-lookup"><span data-stu-id="b2390-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="b2390-109">Kui otsite täielikke märke, kasutage `has` tehtemärki mitte `contains` .</span><span class="sxs-lookup"><span data-stu-id="b2390-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="b2390-110">Saate otsida kindla veeru otsinguid, mitte kõigis veergudes.</span><span class="sxs-lookup"><span data-stu-id="b2390-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="b2390-111">Tabelitega liitumisel Määrake esmalt tabel, kus on vähem ridu.</span><span class="sxs-lookup"><span data-stu-id="b2390-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="b2390-112">`project` ainult teie liitunud tabelite vajalikud veerud.</span><span class="sxs-lookup"><span data-stu-id="b2390-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="b2390-113">Lisateavet leiate teemast [täiustatud jahi päringu parimad tavad](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="b2390-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
