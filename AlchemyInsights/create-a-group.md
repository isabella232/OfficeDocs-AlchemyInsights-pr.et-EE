---
title: Rühma loomine
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816344"
---
# <a name="create-a-group"></a>Rühma loomine

Selles teemas kirjeldatakse rühma loomist.

**Rühma loomise õigus**

Veenduge, et teil oleks õigus luua uus rühm. Üldadministraatorid saavad keelata rühma loomise Azure'i portaalis või Accessi paanil. Võimalik, et vajate uue rühma loomiseks või teile asjakohaste õiguste andmiseks administraatorit.

**Rühma loomise õiguste haldamine**

1. Üldadministraatorid saavad hallata rühma loomise õigusi (turbega seotud põhjustel) või Azure'i portaalis või Accessi paanil loodud Office 365 rühmi, valides jaotises Kõik rühmad Üldine (Sätted) käsu "Kasutajad saavad luua Turberühmi Azure'i portaalides" või "Kasutajad saavad luua Office 365 rühmi Azure'i   >  **portaalides".**
2. Kui teil on Azure Active Directory P1 Premiumi litsents, saate rühma loomist piirata ka kasutajate rühma valimiseks.

**Uute Office 365 rühmaliikmete tervitusteatise keelamine**

Office 365 rühmadesse lisatud kasutajatele saadetava tervitusteatise saab keelata, määrates **PowerShellis Sätte UnifiedGroupWelcomeMessageEnabled** väärtuseks False. Lisateavet selle sätte kohta [leiate siit.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

