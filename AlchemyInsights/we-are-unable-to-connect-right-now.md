---
title: Aktiveerimise probleem – me ei saa kohe ühendust luua
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725979"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 rakenduste parandamine "me ei saa praegu ühendust luua".

Kui teile kuvatakse see teade, proovige teha järgmist.

1. Kontrollige oma tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Lugege teemat [Microsofti URL-ide ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Avage **Start**  >  **Run**ja tippige tekst **Services. msc**. Veenduge, et kõik töötavad järgmised teenused.
    - Võrguga ühendatud seadmete automaatne häälestamine
    - Võrgu loendi teenus
    - Võrgu asukoha teadlikkus
    - Windowsi sündmuste logi

Kui mõni neist teenustest ei tööta, proovige seda käivitada. Kui teil on teenuse käivitamise probleem, käivitage järgmine käsk, avades käsuviiba, kus on kõrgendatud õigused.

**SFC/scannow**

Pärast selle käsu lõpulejõudmist taaskäivitage arvuti.

Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Kui aktiveerite Office ' i Microsoft 365 kaudu, proovige hiljem uuesti](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).