---
title: Office ' i rakenduste parandamine Vabandust, meil on ajutised server Probleemid sõnum
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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764113"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office ' i rakenduste parandamine "Vabandust, meil on ajutised serveriprobleemid" sõnum

Kui kuvatakse see teade, proovige järgmist.

1. Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Office ' i rakendustele Interneti-ühendust. Vaadake [URL-e ja IP-aadresside vahemikku](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. **Start** > **Run**ja seejärel tippige **Services. msc**. Veenduge, et järgmised teenused on kõik töötavad:
    - Võrgu ühendatud seadmed auto-setup
    - Võrguloendi teenus
    - Võrgukoha teadlikkus
    - Windowsi sündmuselogi

Kui üks neist teenustest ei tööta, proovige käivitada. Kui teil on probleem teenuse käivitamine, käivitage järgmine käsk, avades käsuviiba laiendatud õigustega:

**SFC/scannow**

Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.

Üksikasjalikku teavet leiate jaotisest ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovige hiljem uuesti "tõrge, kui aktiveerite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).