---
title: Tingimuslikud Accessi probleemid
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014788"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="0b14e-102">Tingimuslikud Accessi probleemid</span><span class="sxs-lookup"><span data-stu-id="0b14e-102">Conditional access issues</span></span>

<span data-ttu-id="0b14e-103">**Sisselogimise diagnostikaga seotud probleemide lahendamine**</span><span class="sxs-lookup"><span data-stu-id="0b14e-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="0b14e-104">[Sisselogimise diagnostika](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)abil saate kiiresti teada, mis juhtus kasutaja sisselogimisega seotud probleemide või diagnoosimisega.</span><span class="sxs-lookup"><span data-stu-id="0b14e-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="0b14e-105">Käivitage sisselogimise diagnostika.</span><span class="sxs-lookup"><span data-stu-id="0b14e-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="0b14e-106">Analüüsitud sündmuse otsimine, sisestades andmed, mis teil on kasutaja, rakenduse, sisselogimise aja, päringu ID või korrelatsiooni ID-ga.</span><span class="sxs-lookup"><span data-stu-id="0b14e-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="0b14e-107">Vaadake üle diagnostilised tulemid, mis näitavad üksikasju juhtunu kohta ja milliseid toiminguid saab teha muudatuste tegemiseks (kui on vaja muudatusi teha).</span><span class="sxs-lookup"><span data-stu-id="0b14e-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="0b14e-108">**Sisselogimise tõrkeotsingu toimingud**</span><span class="sxs-lookup"><span data-stu-id="0b14e-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="0b14e-109">Liikuge lehele Azure AD sign-in.</span><span class="sxs-lookup"><span data-stu-id="0b14e-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="0b14e-110">Filtreerige sisselogimisi kasutaja, ajavahemikus, rakendus, olek, klientrakendus jne.</span><span class="sxs-lookup"><span data-stu-id="0b14e-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="0b14e-111">Valige sisselogimise sündmus ja vaadake vahekaarti tingimusjuurdepääsu, et näha, milliseid poliitikaid hinnati.</span><span class="sxs-lookup"><span data-stu-id="0b14e-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="0b14e-112">Poliitika üksikasjade kuvamiseks klõpsake poliitika rida ja saage aru, miks see rakendati.</span><span class="sxs-lookup"><span data-stu-id="0b14e-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="0b14e-113">**Tööriistad tingimusliku juurdepääsu poliitika tõrkeotsinguks**</span><span class="sxs-lookup"><span data-stu-id="0b14e-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="0b14e-114">Ainult aruandlusega režiimis saate poliitikaid hinnata, mõjutamata kasutajaid.</span><span class="sxs-lookup"><span data-stu-id="0b14e-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="0b14e-115">Mis-tööriista abil saate simuleerida sisselogimise sündmusi ja vaadata, millist poliitikat kohaldatakse.</span><span class="sxs-lookup"><span data-stu-id="0b14e-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="0b14e-116">Ülevaadete ja aruannete töövihik kuvab iga poliitika reaalajas mõju.</span><span class="sxs-lookup"><span data-stu-id="0b14e-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="0b14e-117">**Baseline Protection poliitika**</span><span class="sxs-lookup"><span data-stu-id="0b14e-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="0b14e-118">Baseline Protection poliitika on aegunud.</span><span class="sxs-lookup"><span data-stu-id="0b14e-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="0b14e-119">Neid ei rakendata enam ja see eemaldatakse peagi Azure ' i portaalist.</span><span class="sxs-lookup"><span data-stu-id="0b14e-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="0b14e-120">Soovitame [turvalisuse vaikesätteid](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)lubada.</span><span class="sxs-lookup"><span data-stu-id="0b14e-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="0b14e-121">Lisateavet tingimusliku juurdepääsu kohta leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="0b14e-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="0b14e-122">[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 tingimusliku juurdepääsu parimad tavad [Tingimustega tingimusjuurdepääsu tingimused](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Juhtelementide kasutamine](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 tingimusjuurdepääsu korral [Asukohad tingimusjuurdepääsu kaudu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="0b14e-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
