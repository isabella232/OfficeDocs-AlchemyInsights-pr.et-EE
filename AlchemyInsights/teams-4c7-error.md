---
title: Meeskonnad 4c7 viga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796072"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 tõrge Microsoft Teamsi

See tõrge ilmneb seetõttu, et Microsoft Teams nõuab vormide autentimist. Kui juurutate Active Directory Federation Services (AD FS), vormide autentimine on lubatud sisevõrgu vaikimisi. Kui Windowsi integreeritud autentimine nurjub, palutakse teil vormide autentimise abil sisse logida.

Selle probleemi lahendamiseks lubage vormide autentimine AD FS Microsofti halduskonsooli (MMC) lisandmooduli abil arvutis, millel on Active Directory kohaliku koopia. Selleks tehke järgmist. 

1. Liikuge navigeerimispaanil **autentimise poliitikad**.
2. Tehke jaotises üksikasjade paanil **toimingud** valik **Redigeeri globaalset esmast autentimist**.
3. Valige vahekaardil **sisevõrgu** **vormide autentimine**.
4. Valige **OK** (või **Rakenda**).