---
title: Microsoft 365 rakenduste parandamine ei leidnud Office ' i litsentsid seotud sõnum
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580437"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 rakenduste kinnitamine "ei leidnud Office ' i litsentsid seotud" sõnum

Kui kuvatakse see teade, proovige järgmist.

1. Kontrollige oma tulemüüri, viirusetõrje tarkvara ja puhverserveri sätteid, et kinnitada, et nad ei blokeeri Interneti-juurdepääsu Microsoft 365 rakendustele. Vt [microsofti 365 URL-id ja IP-aadresside vahemikud](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Eemaldage ja [määrata mõjutatud kasutaja Office ' i litsents](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) . 
3. Avage Office ' i rakendus ja [logige välja](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) kõigist olemasolevatest kasutajakontodest.
4. Avage Windowsi sätted > **kontod**  >  **e-posti & kontod**ja eemaldage kõik töökontod, välja arvatud mõjutatud konto.
5. Avage Windowsi sätted > **kontod**  >  **juurdepääsu töö või kooli**ja katkestada kõik töö kontod, välja arvatud mõjutatud konto.
6. Lähtestage Office ' i aktiveerimisolek. [Õpi, kuidas](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logige sisse](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mõjutatud kasutajakonto abil.

Täiendavate tõrkeotsingulahenduste saamiseks vaadake [Office ' i litsentseerimata toote-ja aktiveerimistõrkeid](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).