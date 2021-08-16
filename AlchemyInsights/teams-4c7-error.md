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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049304"
---
# <a name="4c7-error-in-microsoft-teams"></a>Tõrge 4c7 Microsoft Teams

See tõrge ilmneb seetõttu, Microsoft Teams nõuab vormide autentimist. Teenuse Active Directory Federation Services (AD FS) juurutamisel pole vormide autentimine sisevõrgu jaoks vaikimisi lubatud. Kui Windows nurjub, palutakse teil vormide autentimise abil sisse logida.

Probleemi lahendamiseks lubage vormide autentimine AD FS-i Microsofti halduskonsooli (MMC) lisandmooduli abil arvutis, kus on Active Directory kohalik koopia. Selleks tehke järgmist. 

1. Liikuge navigeerimispaanil sirvides jaotisesse **Autentimispoliitikad.**
2. Valige **üksikasjapaani** jaotises Toimingud käsk **Redigeeri globaalset primaarautentimist**.
3. Valige vahekaardil **Sisevõrk** suvand Vormide **autentimine**.
4. Valige **OK** (või **Rakenda).**