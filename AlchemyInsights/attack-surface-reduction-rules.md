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
# <a name="attack-surface-reduction-rules"></a>Rünnakupinna vähendamise reeglid

Failide või kaustade välistamine võib rünnakupinna vähendamise reeglitega pakutavat kaitset oluliselt vähendada. Failid, mille reegel oleks blokeerinud, on lubatud käivitada ja aruannet ega sündmust ei salvestata. Välistamine kehtib kõigile reeglitele, mis lubavad välistamist.

ASR-i välistamised kasutavad sama süntaksit nagu Microsoft Defenderi viirusetõrje välistamistega. Lisateavet leiate teemast Microsoft Defenderi viirusetõrje kontrolli välistamiste [konfigureerimine ja valideerimine.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Probleemide vältimiseks vaadake läbi levinud vead, [et välistamiste määratlemisel vältida.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Kõik ASR-i reeglid ei toeta välistamist. Kui soovite kontrollida, kas teie reegel toetab välistamist, lugege tabelit [Rünnakupinna vähendamise reeglid.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Rünnakupinna vähendamise reeglid

Teie ettevõtte rünnakupind hõlmab kõiki kohti, kus ründaja võib ettevõtte seadmeid või võrke ohustada. Rünnakupinna vähendamine tähendab organisatsiooni seadmete ja võrgu kaitsmist, mis jätab ründajatele rünnakute sooritamiseks vähem võimalusi. Microsoft Defender for Endpointi ründepinna vähendamise reeglite konfigureerimine võib aidata.

Lisateavet leiate järgmistest teemadest.

- [Asr-i reegli GUID-i vastendamine nimega](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR-i reeglite nõuded:
    - [Windows 10 Pro, versioon 1709 või uuem](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versioon 1709 või uuem](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versioon 1803 (poolaasta-aastane kanal) või uuem versioon](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Õige välistamise tuvastamine

1. Otsige Microsoft-Windows-Windows Defender/Operationali logist sündmuseid 1121 või 1122.

1. Hinnake blokeerimisstsenaariumi ja konteksti ning veenduge, et see stsenaarium tuleb blokeeringust eemaldada.

1. Lugege sündmuse üksikasjades väärtust Tee, mis on välistamist määratlev väärtus.
    - Tehke välistamine võimalikult rangeks.
    - Vajadusel rakendage metamärk (nt asendage muutuja Kasutaja).

1. Rakendage välistamine vastavalt juurutusvajadustele. Lisateavet leiate teemast [Rünnakupinna vähendamise reeglite kohandamine.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Välistamist ei austata

1. Tehke kindlaks, kas reegel toetab välistamist. Lisateavet leiate teemast [Rünnaku pinna vähendamise reeglid.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Vaadake rakendatud välistamised üle ja kontrollige koos sündmuse andmetega kirjavigu või valesti tõlgendatud metamärke. Lisateavet leiate teemast Toetatud [välistamistüübid](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. kui reegli mõju on liiga suur, kaaluge reegli (tagasi) teisaldamist auditirežiimi, et teha täiendav valideerimine. Lisateavet leiate teemast [Microsoft Defender for Endpointi funktsioonide töö testimine auditirežiimis.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Tugiteenuse juhtumi avamiseks koguge tugiteenuseandmeid selle käsu abil.
    
   ** MDEClientAnalyzer.cmd -v**

    Lisateavet leiate teemast Microsoft [Defender for Endpoints'i](issues-with-onboarding-machines.md)pardaseadmetega seotud probleemid.
