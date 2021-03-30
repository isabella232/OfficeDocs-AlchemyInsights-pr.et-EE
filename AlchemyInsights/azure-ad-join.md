---
title: Azure Active Directoryga liitumine
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404594"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="4c5b8-102">Azure Active Directoryga liitumine</span><span class="sxs-lookup"><span data-stu-id="4c5b8-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="4c5b8-103">Kui häälestate seadme registreerimisi esimest korda, veenduge, et olete läbi vaadanud [Azure Active Directorys](/azure/active-directory/devices/overview) seadmehalduse tutvustuse, mis juhendab teid, kuidas azure AD-le seadmed kontrolli alla saada.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="4c5b8-104">Kui registreerite seadmeid otse Azure AD-sse ja registreerite need Intune'i, peate tagama, et [](/mem/intune/fundamentals/licenses-assign) olete [Intune'i](/mem/intune/enrollment/device-enrollment) konfigureerinud ja litsentsimise esmalt paika sidnud.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="4c5b8-105">Veenduge, et teil oleks azure AD-s õigus teha toiminguid.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="4c5b8-106">Ainult Azure AD üldadministraator saab hallata seadme registreerimise sätteid.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="4c5b8-107">Azure AD liitumise rakendamiseks lugege teemat [Azure AD-ühenduse kavandamine.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="4c5b8-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="4c5b8-108">Azure AD-ga liitumise levinumate probleemide lahendamise kohta leiate lisateavet teemast [Azure Ad Joini](/azure/active-directory/devices/faq) KKK ja Windows 10 pro seadme kohta leiate teavet teemast Windows 10 Pro seadmega [Azure AD-ga](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)liitumine – vaja minna üle Microsofti kogukonnale.</span><span class="sxs-lookup"><span data-stu-id="4c5b8-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
