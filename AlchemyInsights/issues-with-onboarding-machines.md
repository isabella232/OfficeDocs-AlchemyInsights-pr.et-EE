---
title: Probleemid arvutite ühendamisel Microsoft Defender for Endpointsiga
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901563"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="76098-102">Probleemid arvutite ühendamisel Microsoft Defender for Endpointsiga</span><span class="sxs-lookup"><span data-stu-id="76098-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="76098-103">Võib-olla on teil probleeme arvutite ühendamisega MDE teenusega.</span><span class="sxs-lookup"><span data-stu-id="76098-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="76098-104">Kui pääsete juurde lõppkasutaja arvutile, tehke järgmist:</span><span class="sxs-lookup"><span data-stu-id="76098-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="76098-105">Laadige alla [MDE kliendianalüsaatori](https://aka.ms/betamdeanalyzer) diagnostika tööriista uusim eelvaate versioon.</span><span class="sxs-lookup"><span data-stu-id="76098-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="76098-106">Paremklõpsake failil **MDEClientAnalyzer.cmd** ja valige käsk "Käivita administraatorina".</span><span class="sxs-lookup"><span data-stu-id="76098-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="76098-107">Järgige juhiseid, mida on soovitatud **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="76098-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="76098-108">Paljusõnaliste logide vaatamiseks vaadake loodud alamkausta nimega **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="76098-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="76098-109">Kui on vaja täiendavaid juhiseid, pöörduge [Microsoft Defender for Endpoint kasutajatoe](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) poole ja esitage analüüsiks fail MDEClientAnalyzerResult.zip.</span><span class="sxs-lookup"><span data-stu-id="76098-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
