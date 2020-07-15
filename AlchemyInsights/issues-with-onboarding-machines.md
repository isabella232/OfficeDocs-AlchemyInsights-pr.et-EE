---
title: Probleemid onboarding masinad
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141464"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="9d513-102">Probleemid onboarding masinad</span><span class="sxs-lookup"><span data-stu-id="9d513-102">Issues with onboarding machines</span></span>

<span data-ttu-id="9d513-103">Teil võib olla probleeme onboarding masinate MDATP teenus.</span><span class="sxs-lookup"><span data-stu-id="9d513-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="9d513-104">Kui pääsete lõppkasutaja arvutisse, toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="9d513-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="9d513-105">Kliendi [ühenduvuse analüsaator](https://aka.ms/mdatpanalyzer) diagnostikatööriista alla laadida.</span><span class="sxs-lookup"><span data-stu-id="9d513-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="9d513-106">Väljavõte ja käivitada MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="9d513-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="9d513-107">Leidke diagnostikalogi kausta nimega MDATPClientAnalyzerResult, sama kausta, kus analüsaator tööriist on alla laaditud.</span><span class="sxs-lookup"><span data-stu-id="9d513-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="9d513-108">Vaadake üle logifail, MDATPClientAnalyzer.txt, et leida ühenduvuse või Interneti puhverserveri sätete probleeme.</span><span class="sxs-lookup"><span data-stu-id="9d513-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>