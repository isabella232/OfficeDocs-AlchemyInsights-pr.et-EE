---
title: EndPoint Manager – turbealused
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420877"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="bddfd-102">EndPoint Manager – turbealused</span><span class="sxs-lookup"><span data-stu-id="bddfd-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="bddfd-103">Turbealused on windowsi sätete eel konfigureeritud rühmad, mis aitavad teil rakendada vastavate turberühmade soovitatud turbesätteid.</span><span class="sxs-lookup"><span data-stu-id="bddfd-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="bddfd-104">Neid alusjooni saab kohandada nii, et need edastaks ainult soovitud sätted ja väärtused.</span><span class="sxs-lookup"><span data-stu-id="bddfd-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="bddfd-105">Lisateavet turbe alusjoonte kohta leiate teemast Windows 10 seadmete konfigureerimine [Intune'i turbe alusjoonte abil.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="bddfd-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="bddfd-106">Praegu on nende toodete jaoks alusjooned.</span><span class="sxs-lookup"><span data-stu-id="bddfd-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="bddfd-107">Windowsi MDM-i turbesätted</span><span class="sxs-lookup"><span data-stu-id="bddfd-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="bddfd-108">Microsoft Defender endPointi turbe jaoks</span><span class="sxs-lookup"><span data-stu-id="bddfd-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="bddfd-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="bddfd-109">Microsoft Edge</span></span>

<span data-ttu-id="bddfd-110">Kõiki lähtejooni värskendatakse perioodiliselt ja need akrementversioonides.</span><span class="sxs-lookup"><span data-stu-id="bddfd-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="bddfd-111">Iga versioon lisab ja eemaldab eelmise versiooni sätted, et veenduda, et alusjoon vastab praegustele juhistele.</span><span class="sxs-lookup"><span data-stu-id="bddfd-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="bddfd-112">Lõpp-punkti turbe turbe võrdluskonsool võimaldab võrrelda erinevaid versioone, muutes muudatused versioonist versiooniks nähtavaks.</span><span class="sxs-lookup"><span data-stu-id="bddfd-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="bddfd-113">Juhised selle kohta, kuidas lähtejoone versiooni kõige tõhusamalt muuta, leiate teemast [Microsoft Intune'i turbe alusprofiilide haldamine.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="bddfd-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="bddfd-114">Pärast turbetaseme juurutamist saate juurutamise olekut jälgida ja sätteid seadme kaupa üle vaadata.</span><span class="sxs-lookup"><span data-stu-id="bddfd-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="bddfd-115">**Märkus.** Lähteandmete aruandluseks võib võtta kuni 24 tundi alates algsest juurutamisest kuni seadmeni ja kuni 6 tundi täiendavate värskenduste saamiseks.</span><span class="sxs-lookup"><span data-stu-id="bddfd-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="bddfd-116">Põhitaseme sätte mittekohanemise kõige levinum põhjus on see, et sama sätet kasutatakse teises profiilis.</span><span class="sxs-lookup"><span data-stu-id="bddfd-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="bddfd-117">Seda stsenaariumi saab konkreetse seadme puhul uurida, valides selle seadme turbe alusjoone profiili sõlmest Seadme olek.</span><span class="sxs-lookup"><span data-stu-id="bddfd-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="bddfd-118">Lisateavet leiate teemast [Konfliktide lahendamine turbe alusjoonte korral.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="bddfd-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>