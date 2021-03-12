---
title: Transpordi reeglite parandamine
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746733"
---
# <a name="fix-transport-rules"></a>Transpordi reeglite parandamine

See sõnum mõjutas kohandatud meilivoo reeglit. Täpse reegli läbivaatamiseks tehke järgmist.

1. Märkige tulemite esitamisel jaotises **Lisateave** üles **GUID** või **poliitika nimi**.
2. Käivitage Exchange Management shell. Lisateavet leiate teemast [Exchange ' i halduse kesta avamine](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Käivitage see käsk (GUID-i abil oma edastusest):  **Get-TransportRule-Identity "GUID" | FL * kirjeldus***
4. Vaadake kirjeldus üle, et näha sõnumit mõjutanud konfigureeritud tingimusi.

Lisateavet leiate teemast [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
