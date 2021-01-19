---
title: Kasutaja sisselogimise tõrked
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900855"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="b1c4e-102">Kasutaja sisselogimise tõrked</span><span class="sxs-lookup"><span data-stu-id="b1c4e-102">User sign-in errors</span></span>

<span data-ttu-id="b1c4e-103">**Sisselogimise diagnostikaga seotud probleemide lahendamine**</span><span class="sxs-lookup"><span data-stu-id="b1c4e-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="b1c4e-104">Kasutaja sisselogimisega seotud probleemide põhjuse või diagnoosimise tuvastamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="b1c4e-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="b1c4e-105">Käivitage [sisselogimise diagnostika](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="b1c4e-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="b1c4e-106">Analüüsitud sündmuse otsimine, sisestades andmed, mis on seotud kasutaja, rakenduse, sisselogimise aja, päringu ID või korrelatsiooni ID-ga.</span><span class="sxs-lookup"><span data-stu-id="b1c4e-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="b1c4e-107">Vaadake üle diagnostilised tulemused, kus on näha, mis juhtus ja milliseid toiminguid saab teha muudatuste tegemiseks, kui on vaja muudatusi teha.</span><span class="sxs-lookup"><span data-stu-id="b1c4e-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="b1c4e-108">**Kas otsite teavet Azure Active Directory (Azure AD) turbelubade teenusest (STS) tagastatud AADSTS tõrkekoodidest?**</span><span class="sxs-lookup"><span data-stu-id="b1c4e-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="b1c4e-109">Lugege [seda artiklit](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , et leida AADSTS, parandusi ja soovitusi.</span><span class="sxs-lookup"><span data-stu-id="b1c4e-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>