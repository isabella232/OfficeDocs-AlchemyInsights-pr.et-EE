---
title: OneDrive sisselogimise tõrge AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112908"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive sisselogimise tõrge AADSTS50011

Kui kuvatakse tõrketeade "AADSTS50011: taotluses määratud vastuse URL ei vasta vastusele" OneDrive rakendusse sisselogimisel kontrollige järgmist.

Teie OneDrive peab olema versiooniga 20.052.XXXX.XXXX võrdne või suurem. Versiooni check to check, click the blue OneDrive icon in the notification area, select **Help & Sätted > Sätted > About**.

Teie võrk võib blokeerida liiklust **g.live.com** ja **oneclient.sfx.ms.** Kui see liiklus on blokeeritud, ei saa OneDrive ise värskendada. Nende URL-ide juurdepääsu tagamiseks tehke koostööd oma võrguadministraatoriga. [Need lõpp-punktid](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) peaksid olema klientidele käeulatuses, kasutades Microsoft 365 plaane.

Kui teil on vaja windowsi praeguse versiooni käsitsi OneDrive, külastage . [https://aka.ms/getonedrive](https://aka.ms/getonedrive)
