---
title: Microsoft 365 rakenduste parandamine Vabandust, meil on ajutine serveri probleemid sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758241"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365 rakenduste parandamine "Kahjuks on meil ajutised serveri probleemid" sõnum

Kui teile kuvatakse see teade, proovige teha järgmist.

1. Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vaadake teemat [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Avage **Start**  >  **Run**ja tippige tekst **Services. msc**. Veenduge, et kõik töötavad järgmised teenused.
    - Võrguga ühendatud seadmete automaatne häälestamine
    - Võrgu loendi teenus
    - Võrgu asukoha teadlikkus
    - Windowsi sündmuste logi

Kui mõni neist teenustest ei tööta, proovige seda käivitada. Kui teil on teenuse käivitamise probleem, käivitage järgmine käsk, avades käsuviiba, kus on kõrgendatud õigused.

**SFC/scannow**

Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.

Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Palun proovi hiljem uuesti, kui aktiveerid](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).