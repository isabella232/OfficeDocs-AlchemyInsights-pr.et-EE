---
title: Aktiveerimisprobleem – me ei saa praegu ühendust luua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716168"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office ' i rakenduste parandamine "me ei saa ühendust kohe" sõnum

Kui kuvatakse see teade, proovige järgmist.

1. Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Office ' i rakendustele Interneti-ühendust. Vaadake [Microsofti URL-e ja IP-aadresside vahemikku](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. **Start** > **Run**ja seejärel tippige **Services. msc**. Veenduge, et järgmised teenused on kõik töötavad:
    - Võrgu ühendatud seadmed auto-setup
    - Võrguloendi teenus
    - Võrgukoha teadlikkus
    - Windowsi sündmuselogi

Kui üks neist teenustest ei tööta, proovige käivitada. Kui teil on probleem teenuse käivitamine, käivitage järgmine käsk, avades käsuviiba laiendatud õigustega:

**SFC/scannow**

Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.

Üksikasjalikku teavet leiate jaotisest ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovige hiljem uuesti "tõrge, kui aktiveerite Office ' i Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).