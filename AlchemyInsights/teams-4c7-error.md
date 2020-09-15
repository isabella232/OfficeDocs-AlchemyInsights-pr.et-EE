---
title: Teamsi 4c7 tõrge
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700199"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teamsi 4c7 tõrge

See tõrge ilmneb, sest Microsoft Teamsi jaoks on vaja vorme autentida. Kui juurutate Active Directory Federation Services (AD FS), pole vormide autentimine vaikimisi sisevõrgu jaoks lubatud. Kui Windowsi integreeritud autentimine nurjub, palutakse teil vormide autentimise abil sisse logida.

Selle probleemi lahendamiseks lubage vormide autentimine, kasutades AD FS-i Microsoft Management Console (MMC) lisandmoodulit arvutis, kus on Active Directory kohalik koopia. Selleks tehke järgmist. 

1. Liikuge navigeerimispaanil sirvides **autentimise poliitikale**.
2. Valige üksikasjade paani jaotises **toimingud** nupp **Redigeeri globaalset esmast autentimist**.
3. Valige vahekaardil **sisevõrk** suvand **vormide autentimine**.
4. Valige **OK** (või **Rakenda**).