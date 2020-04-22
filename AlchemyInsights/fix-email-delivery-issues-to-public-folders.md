---
title: Meililoaga avalike kaustade e-posti kohaletoimetamise probleemide lahendamine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716348"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Meililoaga avalike kaustade e-posti kohaletoimetamise probleemide lahendamine

Kui välised saatjad ei saa saata sõnumeid meililoaga ühiskaustade ja saatjate kuvatakse tõrge: **ei leitud (550 5.4.1)**, veenduge, et ühiskausta e-posti domeen on konfigureeritud SISEMINE relee domeeni asemel autoriteetse domeeni:

1. Avage [Exchange ' i halduskeskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Avage **meilivoog** \> **aktsepteeritud domeenid**, valige aktsepteeritud domeen ja klõpsake **redigeerida**.

3. Atribuutide lehel, mis avaneb, kui domeeni tüüp on seatud **autoriteetne**, muutke **sisemise relee** väärtuseks ja klõpsake siis nuppu **Salvesta**.

Kui välised saatjad kuvatakse tõrge **teil pole õigust (550 5.7.13)**, käivitage järgmine käsk [Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) ühiskausta anonüümsete kasutajate õiguste nägemiseks:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Näiteks `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Lubada väliste kasutajate saata e-posti ühiskausta, lisage CreateItems juurdepääsu õigus kasutaja anonüümne. Näiteks `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
