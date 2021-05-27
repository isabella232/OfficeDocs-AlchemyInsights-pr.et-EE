---
title: Rünnakupinna vähendamise reeglid
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676229"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c9951-102">Rünnakupinna vähendamise reeglid</span><span class="sxs-lookup"><span data-stu-id="c9951-102">Attack surface reduction rules</span></span>

<span data-ttu-id="c9951-103">Failide või kaustade välistamine võib rünnakupinna vähendamise reeglitega pakutavat kaitset oluliselt vähendada.</span><span class="sxs-lookup"><span data-stu-id="c9951-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="c9951-104">Failid, mille reegel oleks blokeerinud, on lubatud käivitada ja aruannet ega sündmust ei salvestata.</span><span class="sxs-lookup"><span data-stu-id="c9951-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="c9951-105">Välistamine kehtib kõigile reeglitele, mis lubavad välistamist.</span><span class="sxs-lookup"><span data-stu-id="c9951-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="c9951-106">ASR-i välistamised kasutavad sama süntaksit nagu Microsoft Defenderi viirusetõrje välistamistega.</span><span class="sxs-lookup"><span data-stu-id="c9951-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="c9951-107">Lisateavet leiate teemast Microsoft Defenderi viirusetõrje kontrolli välistamiste [konfigureerimine ja valideerimine.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c9951-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="c9951-108">Probleemide vältimiseks vaadake läbi levinud vead, [et välistamiste määratlemisel vältida.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c9951-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c9951-109">Kõik ASR-i reeglid ei toeta välistamist.</span><span class="sxs-lookup"><span data-stu-id="c9951-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="c9951-110">Kui soovite kontrollida, kas teie reegel toetab välistamist, lugege tabelit [Rünnakupinna vähendamise reeglid.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c9951-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c9951-111">Rünnakupinna vähendamise reeglid</span><span class="sxs-lookup"><span data-stu-id="c9951-111">Attack surface reduction rules</span></span>

<span data-ttu-id="c9951-112">Teie ettevõtte rünnakupind hõlmab kõiki kohti, kus ründaja võib ettevõtte seadmeid või võrke ohustada.</span><span class="sxs-lookup"><span data-stu-id="c9951-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="c9951-113">Rünnakupinna vähendamine tähendab organisatsiooni seadmete ja võrgu kaitsmist, mis jätab ründajatele rünnakute sooritamiseks vähem võimalusi.</span><span class="sxs-lookup"><span data-stu-id="c9951-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="c9951-114">Microsoft Defender for Endpointi ründepinna vähendamise reeglite konfigureerimine võib aidata.</span><span class="sxs-lookup"><span data-stu-id="c9951-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="c9951-115">Lisateavet leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="c9951-115">For more information, see:</span></span>

- [<span data-ttu-id="c9951-116">Asr-i reegli GUID-i vastendamine nimega</span><span class="sxs-lookup"><span data-stu-id="c9951-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="c9951-117">ASR-i reeglite nõuded:</span><span class="sxs-lookup"><span data-stu-id="c9951-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="c9951-118">Windows 10 Pro, versioon 1709 või uuem</span><span class="sxs-lookup"><span data-stu-id="c9951-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c9951-119">Windows 10 Enterprise, versioon 1709 või uuem</span><span class="sxs-lookup"><span data-stu-id="c9951-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c9951-120">Windows Server, versioon 1803 (poolaasta-aastane kanal) või uuem versioon</span><span class="sxs-lookup"><span data-stu-id="c9951-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="c9951-121">Õige välistamise tuvastamine</span><span class="sxs-lookup"><span data-stu-id="c9951-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="c9951-122">Otsige Microsoft-Windows-Windows Defender/Operationali logist sündmuseid 1121 või 1122.</span><span class="sxs-lookup"><span data-stu-id="c9951-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="c9951-123">Hinnake blokeerimisstsenaariumi ja konteksti ning veenduge, et see stsenaarium tuleb blokeeringust eemaldada.</span><span class="sxs-lookup"><span data-stu-id="c9951-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="c9951-124">Lugege sündmuse üksikasjades väärtust Tee, mis on välistamist määratlev väärtus.</span><span class="sxs-lookup"><span data-stu-id="c9951-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="c9951-125">Tehke välistamine võimalikult rangeks.</span><span class="sxs-lookup"><span data-stu-id="c9951-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="c9951-126">Vajadusel rakendage metamärk (nt asendage muutuja Kasutaja).</span><span class="sxs-lookup"><span data-stu-id="c9951-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="c9951-127">Rakendage välistamine vastavalt juurutusvajadustele.</span><span class="sxs-lookup"><span data-stu-id="c9951-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="c9951-128">Lisateavet leiate teemast [Rünnakupinna vähendamise reeglite kohandamine.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="c9951-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="c9951-129">Välistamist ei austata</span><span class="sxs-lookup"><span data-stu-id="c9951-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="c9951-130">Tehke kindlaks, kas reegel toetab välistamist.</span><span class="sxs-lookup"><span data-stu-id="c9951-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="c9951-131">Lisateavet leiate teemast [Rünnaku pinna vähendamise reeglid.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c9951-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="c9951-132">Vaadake rakendatud välistamised üle ja kontrollige koos sündmuse andmetega kirjavigu või valesti tõlgendatud metamärke.</span><span class="sxs-lookup"><span data-stu-id="c9951-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="c9951-133">Lisateavet leiate teemast Toetatud [välistamistüübid](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="c9951-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="c9951-134">kui reegli mõju on liiga suur, kaaluge reegli (tagasi) teisaldamist auditirežiimi, et teha täiendav valideerimine.</span><span class="sxs-lookup"><span data-stu-id="c9951-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="c9951-135">Lisateavet leiate teemast [Microsoft Defender for Endpointi funktsioonide töö testimine auditirežiimis.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="c9951-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="c9951-136">Tugiteenuse juhtumi avamiseks koguge tugiteenuseandmeid selle käsu abil.</span><span class="sxs-lookup"><span data-stu-id="c9951-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="c9951-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="c9951-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="c9951-138">Lisateavet leiate teemast Microsoft [Defender for Endpoints'i](issues-with-onboarding-machines.md)pardaseadmetega seotud probleemid.</span><span class="sxs-lookup"><span data-stu-id="c9951-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
