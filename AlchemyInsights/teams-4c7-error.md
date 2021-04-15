---
title: Teams 4c7 tõrge
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786665"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 tõrge Microsoft Teamsis

See tõrge ilmneb seetõttu, et Microsoft Teams nõuab vormide autentimist. Teenuse Active Directory Federation Services (AD FS) juurutamisel pole vormide autentimine sisevõrgu jaoks vaikimisi lubatud. Kui Windowsi integreeritud autentimine nurjub, palutakse teil vormide autentimise abil sisse logida.

Probleemi lahendamiseks lubage vormide autentimine AD FS-i Microsofti halduskonsooli (MMC) lisandmooduli abil arvutis, kus on Active Directory kohalik koopia. Selleks tehke järgmist. 

1. Liikuge navigeerimispaanil sirvides jaotisesse **Autentimispoliitikad.**
2. Valige **üksikasjapaani** jaotises Toimingud käsk **Redigeeri globaalset primaarautentimist**.
3. Valige vahekaardil **Sisevõrk** suvand Vormide **autentimine**.
4. Valige **OK** (või **Rakenda).**