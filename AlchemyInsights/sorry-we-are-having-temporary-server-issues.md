---
title: Rakenduste Microsoft 365 Kahjuks on meil ajutiste serveriprobleemide teade
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021592"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Tõrketeade Microsoft 365 "Kahjuks on meil ajutised serveriprobleemid".

Kui teile kuvatakse see teade, proovige järgmist.

1. Kontrollige tulemüüri, viirusetõrjetarkvara ja puhverserveri sätteid, et veenduda, et need ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vt [URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Avage Start Run  >  **(Käivita)** ja seejärel tippige **services.msc**. Veenduge, et kõik järgmised teenused töötaks.
    - Võrguühendusega seadmete automaathäälestus
    - Võrguteenus
    - Võrguasukoha teadlikkus
    - Windows Sündmuselogi

Kui mõni neist teenustest ei tööta, proovige seda käivitada. Kui teil on teenuse käivitamisel probleeme, käivitage järgmine käsk, avades administraatoriõigustega käsuviiba.

**sfc /scannow**

Pärast selle käsu lõpule viimist taaskäivitage arvuti.

Üksikasjalikku teavet leiate teemast ["Kahjuks ei saa me teie kontoga ühendust luua. Proovige hiljem uuesti" tõrge, kui aktiveerite](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).