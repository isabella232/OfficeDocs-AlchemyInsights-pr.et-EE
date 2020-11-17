---
title: Rühma loomine
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088689"
---
# <a name="create-a-group"></a>Rühma loomine

Selles teemas kirjeldatakse rühma loomist.

**Rühma loomise õigus**

Veenduge, et teil on õigus luua uus rühm. Globaalsed administraatorid saavad rühma loomise keelata Azure ' i portaalis või Accessi paanil. Teil võib olla vaja administraatorit, et luua uus rühm või anda teile vastavad õigused.

**Rühma loomise õiguse haldamine**

1. Globaalsed administraatorid saavad hallata Azure ' i portaalis või Accessi paneelis loodud rühma loomise õiguseid (turbega seotud põhjustel) või Office 365 rühmi, valides "kasutajad saavad luua turberühma Azure ' i portaalis" või "kasutajad saavad luua Office 365 rühmi Azure ' i portaalis" **kõigi rühmade**  >  **üldised suvandid (sätted)**.
2. Kui teil on Azure Active Directory P1 Premiumi litsents, saate rühma loomist piirata ka kasutajate rühma valimiseks.

**Uute Office 365 rühma liikmete jaoks tervitusprogrammi teatise keelamine**

Office 365 rühmadesse lisatud kasutajatele, kes on lisatud Office rühmadesse, saab keelata, kui säte **UnifiedGroupWelcomeMessageEnabled** on PowerShellis FALSE. [Siit](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)saate teada, kuidas see säte käib.

