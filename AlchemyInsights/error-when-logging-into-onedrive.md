---
title: 0x8004de40 OneDrive'i käivitamisel ilmnes tõrge
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813648"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 OneDrive'i käivitamisel ilmnes tõrge

Kui **OneDrive'0x8004de40** sisselogimisel kuvatakse tõrketeade, taaskäivitage arvuti töö- või koolidomeeniga ühenduse loomise ajal. Kui teile kuvatakse see tõrge pärast taaskäivitamist, proovige seda töö- või koolidomeeniga ühenduse saamisel.

1. Klõpsake nuppu Start ja  tippige **otsinguväljale tekst cmd** või käsuviip, paremklõpsake käsuviiba rakendust ja valige **Käivita administraatorina**. Kui teilt küsitakse administraatoriparooli või kinnitust, tippige parool või klõpsake nuppu **Luba**.  

2. Tippige aknas Käsuviip **tekst dsregcmd /leave**  ja oodake, kuni käsk lõpule jõuaks. Seejärel tippige **dsregcmd /join** ja oodake, kuni käsk on lõpule viidud.
3. Taaskäivitage arvuti.
