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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929301"
---
# <a name="create-a-group"></a>Rühma loomine

Selles teemas kirjeldatakse rühma loomist.

**Rühma loomise õigus**

Veenduge, et teil oleks õigus luua uus rühm. Üldadministraatorid saavad keelata rühma loomise Azure'i portaalis või Accessi paanil. Võimalik, et vajate uue rühma loomiseks või teile asjakohaste õiguste andmiseks administraatorit.

**Rühma loomise õiguste haldamine**

1. Üldadministraatorid saavad hallata rühma loomise õigusi (turbega seotud põhjustel) või azure'i portaalis või Accessi paanil loodud Office 365-rühmi, valides jaotises Kõik rühmad Üldine (Sätted) käsu "Kasutajad saavad azure'i portaalides turberühmi luua" või "Kasutajad saavad luua Office 365-rühmi  >  **Azure'i portaalides".**
2. Kui teil on P1 Azure Active Directory Premium, saate rühma loomist piirata ka rühma valimiseks.

**Uute rühmaliikmete tervitusteatise Office 365 keelamine**

Kui tervitusteatis saadetakse kasutajatele, kes Office 365 rühmadesse, saab keelata, määrates **PowerShellis Sätte UnifiedGroupWelcomeMessageEnabled** väärtuseks False. Lisateavet selle sätte kohta [leiate siit.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

