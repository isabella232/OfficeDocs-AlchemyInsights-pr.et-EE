---
title: Tervitusteade Microsoft 365 rühmad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357538"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Tervitusteade Microsoft 365 rühmad

Uued kasutajad, kes ühinevad Microsoft 365 rühma saavad teretulnud e-posti kui "UnifiedGroupWelcomeMessageEnabled" atribuut on tõene.

Kui soovite keelata tervitussõnumi, kasutage järgmist [EXO PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) käsk:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
