---
title: E-posti kohaletoimetamise lahendamine meililoaga Ühiskaustad
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525096"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>E-posti kohaletoimetamise lahendamine meililoaga Ühiskaustad

Kui välistelt saatjatelt ei saa sõnumeid saata meililoaga avalike kaustade ja nende saatjad saavad viga: **ei suutnud leida (550 5.4.1)**, kontrollige e-posti domeeni jaoks ühiskaust on konfigureeritud sisemiseks vahedomeeniks asemel on autoriteetne Domeen:

1. Avage [Exchange'i administraatori center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Mine **meilivoo** \> **aktsepteeritud domeenid**, valige aktsepteeritud ja klõpsake siis nuppu **Redigeeri**.

3. Atribuutide lehekülg avaneb, kui domeeni tüüp väärtuseks **Authoritative**, muutke **sisemiseks** vahedomeeniks ja klõpsake siis nuppu **Salvesta**.

Kui välised saatjad saavad viga, **teil ei ole õigust (550 5.7.13)**, käivitage järgmine käsk [Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) näha ühiskausta anonüümsete kasutajate õigused:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Näiteks `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Väliskasutajatele tuleks saada-seda ühiskausta, lisada CreateItems juurdepääs otse kasutaja Anonymous. Näiteks `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
