---
title: OneDrive ' i käivitamisel ilmneb 0x8004de40 tõrge
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823018"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>OneDrive ' i käivitamisel ilmneb 0x8004de40 tõrge

Kui OneDrive ' i sisselogimisel ilmneb tõrge **0x8004de40** , taaskäivitage arvuti töö või kooli domeeniga ühendatud. Kui tõrketeade kuvatakse pärast taaskäivitamist, proovige seda siis, kui olete oma töö või kooli domeeniga ühendatud.

1. Klõpsake nuppu Start ja **Tippige väljale Otsing** tekst **cmd** või Käsuviip, paremklõpsake käsuviiba rakendust ja valige **Käivita administraatorina** . Kui teilt küsitakse administraatori parooli või kinnitust, tippige parool või klõpsake nuppu **Luba** .  

2. Tippige käsuviiba aknas **dsregcmd/Leave**  ja oodake, kuni käsk on täidetud. Seejärel tippige **dsregcmd/JOIN** ja oodake, kuni käsk on täidetud.
3. Taaskäivitage arvuti.
