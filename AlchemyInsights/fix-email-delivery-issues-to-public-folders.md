---
title: Meiliedastusprobleemide lahendamine meili toega avalikele kaustadele
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068808"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Meiliedastusprobleemide lahendamine meili toega avalikele kaustadele

Kui välised saatjad ei saa teie meili toega avalikele kaustadele sõnumeid saata ja saatjatele kuvatakse tõrketeade: seda ei leitud **(550 5.4.1),** veenduge, et avaliku kausta meilidomeen on konfigureeritud autoriteetse domeeni asemel sisevahendusdomeen domeenina.

1. Avage [Exchange halduskeskus (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Avage **Meilivoog** \> **Aktsepteeritud domeenid**, valige aktsepteeritud domeen ja seejärel klõpsake nuppu **Redigeeri.**

3. Kui avataval atribuutide lehel on domeenitüübiks määratud **Autoriteetne,** määrake väärtuseks **Sisemine edastamine ja** seejärel klõpsake nuppu **Salvesta**.

Kui välistele saatjatele kuvatakse tõrge, mis teil pole **õigust (550 5.7.13),** [käivitage Exchange Online PowerShellis](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) järgmine käsk, et näha anonüümsete kasutajate õigusi avalikus kaustas.

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Näiteks `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Kui soovite, et väliskasutajad saavad sellele avalikule kaustale meilisõnumeid saata, lisage createitems-juurdepääs otse kasutajale Anonüümne. Näiteks `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
