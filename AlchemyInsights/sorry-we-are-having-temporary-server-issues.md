---
title: Microsoft 365 rakenduste parandamine Vabandust, meil on ajutised server Probleemid sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582699"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365 rakenduste parandamine "Vabandust, meil on ajutised serveri probleemid" sõnum

Kui kuvatakse see teade, proovige järgmist.

1. Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vaadake [URL-e ja IP-aadresside vahemikku](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. **Start**  >  **Run**ja seejärel tippige **Services. msc**. Veenduge, et järgmised teenused on kõik töötavad:
    - Võrgu ühendatud seadmed auto-setup
    - Võrguloendi teenus
    - Võrgukoha teadlikkus
    - Windowsi sündmuselogi

Kui üks neist teenustest ei tööta, proovige käivitada. Kui teil on probleem teenuse käivitamine, käivitage järgmine käsk, avades käsuviiba laiendatud õigustega:

**SFC/scannow**

Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.

Üksikasjalikku teavet leiate jaotisest ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovige hiljem uuesti "tõrge, kui aktiveerite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).