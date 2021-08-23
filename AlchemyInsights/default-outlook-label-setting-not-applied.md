---
title: Sildi Outlook pole rakendatud
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454566"
---
# <a name="default-outlook-label-setting-not-applied"></a>Sildi Outlook pole rakendatud

Kui teie Outlook vaikesildisätted ei rakendata õigesti ja mõni muu silt või silti ei rakendata, võib teil esineda teadaolev probleem (MC277818) ja peaksite probleemi lahendamiseks tegema ühte neist 2 võimalusest.

**1. võimalus.**

1. Avage Microsoft 365 vastavuskeskus > lahenduste   >  **teabekaitse**.
1. Valige **Sildipoliitikad** ja valige redigeeritav sildipoliitika (**OutlookDefaultlabeli** säte pole kõnealuse sildipoliitika jaoks õigesti määratud. Käivitage **selle sätte vaatamiseks Get-labelpolicy** ja seejärel valige **Redigeeri poliitikat.**
1. Valige **Edasi,** kuni kuvatakse säte **Rakenda** see vaikesilt meilisõnumitele, mis on saadaval, kui valite dialoogiboksis Poliitikasätted ruudu Nõua kasutajatelt silti pärija meilisõnumitele ja **dokumentidele.** 
1. Valige **dialoogiboksis Dokumentidele vaikesildi** lisamine **ripploendist** Väärtus Pole.
1. Sildisätete **salvestamiseks valige Edasi** ja Edasta. 

**2. võimalus.**

Turbe- [ja vastavuskeskuse Powershellis](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)saate käsu Set-LabelPolicy **outlookDefaultlabel** muuta  üksuses {OutlookDefaultLabel="None"} käsuks Pole.

Käivita: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Lisateavet selle kohta, kuidas Outlook vaikesildid, leiate [teemast](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)Outlook.