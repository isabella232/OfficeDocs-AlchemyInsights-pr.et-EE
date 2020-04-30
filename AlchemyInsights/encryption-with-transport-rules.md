---
title: Krüptimine transpordireeglitega
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915086"
---
# <a name="encryption-with-transport-rules"></a>Krüptimine transpordireeglitega

[Exchange’i halduskeskuses](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) saate meilivoo reeglites kasutada meilisõnumite krüptimise käivitamiseks Office’i sõnumikrüptimine (OME) funktsioone. Valige transpordireegli tingimuses suvand **Rakenda Office 365 sõnumikrüptimine ja õiguste kaitse**.

- Lisateavet vaadake teemast [Meilivoo reegli krüptimiseks määratlemine](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Kasutage PowerShellis cmlet-käsku [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) ja määrake parameeter *ApplyOME* väärtusele $true.
