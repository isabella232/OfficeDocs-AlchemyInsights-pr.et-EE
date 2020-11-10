---
title: OneDrive ' i sisselogimise tõrge AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982448"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive ' i sisselogimise tõrge AADSTS50011

Kui kuvatakse tõrketeade "AADSTS50011: taotluses määratud vastuse URL ei vasta vastusele" OneDrive ' i rakendusse sisselogimisel, kontrollige järgmist.

Teie OneDrive ' i versioon peab olema võrdne või suurem kui versioon 20.052. XXXX. XXXX. Oma versiooni kontrollimiseks klõpsake olekualal sinise OneDrive ' i ikooni, valige **spikker & sätted > sätted >**.

Teie võrk võib blokeerida liiklust **g.live.com** ja **oneclient.SFX.MS**. Kui see liiklus on blokeeritud, ei saa OneDrive ennast värskendada. Töötage oma võrguadministraatoriga, et tagada juurdepääs nendele URL-idele. [Need lõpp-punktid](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) peavad olema juurdepääsetavad klientidele, kes kasutavad Microsoft 365 lepinguid.

Kui teil on vaja käsitsi hankida OneDrive ' i praegune versioon, külastage veebilehte [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
