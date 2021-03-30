---
title: Autentimisrakendus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404599"
---
# <a name="authentication-app"></a><span data-ttu-id="7a82f-102">Autentimisrakendus</span><span class="sxs-lookup"><span data-stu-id="7a82f-102">Authentication app</span></span>

<span data-ttu-id="7a82f-103">Kui olete üldadministraator, saate sisselogimisdiagnostika abil kiiresti teada saada, mis juhtus või diagnoosida kasutaja [sisselogimisega seotud probleeme.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="7a82f-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="7a82f-104">Käivitage diagnostika, klõpsates nuppu["Käivita diagnostika".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="7a82f-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="7a82f-105">Uurige analüüsitav sündmus, sisestades kasutaja, rakenduse, sisselogimisaja, päringu ID või korrelatsiooni ID üksikasjad.</span><span class="sxs-lookup"><span data-stu-id="7a82f-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="7a82f-106">Vaadake üle diagnostikatulemid, kus on kuvatud üksikasjad selle kohta, mis juhtus ja milliseid toiminguid saate muudatuste vaatamiseks teha ( kui on vaja teha muudatusi).</span><span class="sxs-lookup"><span data-stu-id="7a82f-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="7a82f-107">**Kontrollige, mis on rakendatav.**</span><span class="sxs-lookup"><span data-stu-id="7a82f-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="7a82f-108">Kui kasutaja ei saa rakenduses Microsoft Authenticator tõuketeatist, veenduge, et neid ei kuvata MFA blokeeritud kasutajate all, nagu on kirjeldatud jaotises Kasutajate [blokeerimine ja blokeeringu blokeerimine.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="7a82f-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="7a82f-109">Kui kasutaja ei blokeeri MFA-d, kuid ei saa tõuketeatist, saab ta avada Rakenduse Microsoft Authenticator, mis võtab ootel kinnitamise taotlused.</span><span class="sxs-lookup"><span data-stu-id="7a82f-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="7a82f-110">Alternatiivse sisselogimisviisina saab kasutaja klõpsata ka nuppu Logi sisse muul viisil ja valida mobiilirakenduse kinnituskoodi.</span><span class="sxs-lookup"><span data-stu-id="7a82f-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="7a82f-111">Microsoft Authenticatori rakendus on ainus saadaval meetod paljude kasutajate jaoks.</span><span class="sxs-lookup"><span data-stu-id="7a82f-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="7a82f-112">[Lugege lisateavet turbe vaikesätete kohta,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)vaadake [korduma kippuvate](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) küsimuste ja nende lahendamise kohta authenticatori rakenduse KKK-d.</span><span class="sxs-lookup"><span data-stu-id="7a82f-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="7a82f-113">**Soovitatavad videod**</span><span class="sxs-lookup"><span data-stu-id="7a82f-113">**Recommended Videos**</span></span>

<span data-ttu-id="7a82f-114">[Authenticatori rakenduse häälestamine uues telefonis (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="7a82f-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
