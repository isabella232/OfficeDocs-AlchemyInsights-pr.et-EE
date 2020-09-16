---
title: OneDrive ' i 0x8004de40 lahendamise tõrge
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745126"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive ' i 0x8004de40 lahendamise tõrge

Kui OneDrive ' iga kuvatakse 0x8004de40 tõrge, tehke järgmist.

- Taaskäivitage mõjutatud arvuti, kui olete ühendatud oma Acitve kataloogiteenuse domeeniga.
- Kui taaskäivitamine probleemi ei lahenda, liituge oma seadmega Azure AD. 

**Märkus**: te peate nende toimingute tegemisel olema ettevõtte võrgus. Ärge tehke neid toiminguid, kui te ei saa luua ühendust oma ettevõtte infrastruktuuriga (nt reisil olles). 

- Avage tõstetud Käsuviip. 
- Kõrgenenud käsuviiba avamiseks klõpsake nuppu **Start**, paremklõpsake käsku **Käsuviip**ja seejärel klõpsake käsku **Käivita administraatorina**.
- Tippige *dsregcmd/Leave* ja vajutage sisestusklahvi ( **Enter)**.
- Kui olete lõpetanud, tippige *dsregcmd/JOIN* ja vajutage sisestusklahvi ( **Enter)**.
- Kui olete lõpetanud, sulgege Käsuviip.
- Taaskäivitage arvuti ja logige sisse OneDrive ' i.