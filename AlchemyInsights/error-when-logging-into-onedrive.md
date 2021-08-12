---
title: 0x8004de40 käivitamisel OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946575"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 käivitamisel OneDrive

Kui teile kuvatakse tõrketeade **0x8004de40** sisselogimisel, OneDrive arvuti töö- või koolidomeeniga ühenduse loomise ajal taaskäivitada. Kui teile kuvatakse see tõrge pärast taaskäivitamist, proovige seda töö- või koolidomeeniga ühenduse saamisel.

1. Klõpsake nuppu Start ja  tippige **otsinguväljale tekst cmd** või käsuviip, paremklõpsake käsuviiba rakendust ja valige **Käivita administraatorina**. Kui teilt küsitakse administraatoriparooli või kinnitust, tippige parool või klõpsake nuppu **Luba**.  

2. Tippige aknas Käsuviip **tekst dsregcmd /leave**  ja oodake, kuni käsk lõpule jõuaks. Seejärel tippige **dsregcmd /join** ja oodake, kuni käsk on lõpule viidud.
3. Taaskäivitage arvuti.
