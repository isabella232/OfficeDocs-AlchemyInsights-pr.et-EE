---
title: Meilisõnumite kohaletoimetamisega seotud probleemide lahendamine meililoaga ühiskaustade korral
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366460"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Meilisõnumite kohaletoimetamisega seotud probleemide lahendamine meililoaga ühiskaustade korral

Kui välised saatjad ei saa saata meilisõnumeid teie meililoaga ühiskaustu ja saatjad saavad tõrketeate: **ei leita (550 5.4.1)**, veenduge, et ühiskausta Domeen oleks konfigureeritud autoriteetse domeeni asemel asutusesiseseks edastamise domeeniks.

1. Avage [Exchange ' i halduskeskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Avage jaotis **meilivoo** \> **aktsepteeritud domeenid**, valige aktsepteeritud domeen ja klõpsake nuppu **Redigeeri**.

3. Kui domeeni tüüp on seatud **autoriteetseks**, muutke kuvatavas atribuutide lehel väärtust **sisemine edastus** ja seejärel klõpsake nuppu **Salvesta**.

Kui välised saatjad saavad tõrketeate **(550 5.7.13)**, käivitage [Exchange Online PowerShellis](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) järgmine käsk, et kuvada anonüümsete kasutajate õigused avalikus kaustas.

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Näiteks `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Kui soovite, et väliskasutajad saaksid selle ühiskausta meilisõnumeid saata, lisage CreateItems juurdepääs otse kasutajale anonüümseks. Näiteks `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
