---
title: EndPoint Manager – turbe etalonid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440880"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="b78d6-102">EndPoint Manager – turbe etalonid</span><span class="sxs-lookup"><span data-stu-id="b78d6-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="b78d6-103">Turbe etalonid on Windowsi sätete eelkonfigureeritud rühmad, mis aitavad teil neid asjaomaste turvalisuse töörühmade soovitatavaid turvalisuse seadistusi rakendada.</span><span class="sxs-lookup"><span data-stu-id="b78d6-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="b78d6-104">Neid etalone saab kohandada, et pakkuda ainult soovitud seadistusi ja väärtusi.</span><span class="sxs-lookup"><span data-stu-id="b78d6-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="b78d6-105">Lisateavet turbe etalonide kohta vaadake teemast [Intune’is Windows 10 seadmete konfigureerimiseks turbe etalonide kasutamine](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="b78d6-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="b78d6-106">Nende toodete praegused etalonid on järgmised.</span><span class="sxs-lookup"><span data-stu-id="b78d6-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="b78d6-107">Windows MDM-i turbesätted</span><span class="sxs-lookup"><span data-stu-id="b78d6-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="b78d6-108">Microsoft Defender for Endpointi turve</span><span class="sxs-lookup"><span data-stu-id="b78d6-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="b78d6-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b78d6-109">Microsoft Edge</span></span>

<span data-ttu-id="b78d6-110">Kõiki etalone värskendatakse perioodiliselt ja antakse välja astmeliste versioonidena.</span><span class="sxs-lookup"><span data-stu-id="b78d6-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="b78d6-111">Iga versioon lisab ja/või eemaldab eelmise versiooni sätted, et tagada, et etalon vastaks praegustele juhistele.</span><span class="sxs-lookup"><span data-stu-id="b78d6-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="b78d6-112">Lõpp-punkti turvalisuse turbe etalonide konsool võimaldab võrrelda erinevaid versioone, muutes versioonide vahelised muudatused nähtavaks.</span><span class="sxs-lookup"><span data-stu-id="b78d6-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="b78d6-113">Juhisteks selle kohta, kuidas saab kõige tõhusamalt muuta seda, milline lähtealuse versioon juurutatakse, vaadake teemast [Turbe etaloni profiilide haldamine Microsoft Intune’is](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="b78d6-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="b78d6-114">Turbe etaloni juurutamise järel saate jälgida juurutamise olekut ja vaadata üle seadmepõhiselt seadistused.</span><span class="sxs-lookup"><span data-stu-id="b78d6-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="b78d6-115">**Märkus.** Etalonide aruandluse andmete ilmumiseks võib kuluda kuni 24 tundi alates algsest seadmes juurutamisest ja kuni 6 tundi edasiste värskenduste korral.</span><span class="sxs-lookup"><span data-stu-id="b78d6-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="b78d6-116">Etaloni seadistuse mitte rakendumise kõige levinum põhjus on, kui erinev profiil kasutab sama seadistust.</span><span class="sxs-lookup"><span data-stu-id="b78d6-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="b78d6-117">Seda stsenaariumit saab konkreetse seadme jaoks uurida, valides selle seadme turbe etaloni profiili sõlmest Seadme olek.</span><span class="sxs-lookup"><span data-stu-id="b78d6-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="b78d6-118">Üksikasju vaadake teemast [Turbe etalonide konfliktide lahendamine](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="b78d6-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>