---
title: Karantiinis puuduvad e-kirjad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569048"
---
# <a name="missing-emails-in-quarantine"></a>Karantiinis puuduvad meilid "

Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Turvalisuse & vastavuse keskuse avamiseks [https://protection.office.com](https://protection.office.com/) . Otse karantiini lehe avamiseks [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Saate otsida järgmiste väärtuste järgi:  

- **Sõnumi ID**: globaalne kordumatu identifikaator. Kui valite loendist sõnumi, kuvatakse kuvatava **üksikasjade** hüpik- **sõnumi ID** väärtus. Administraatorid saavad kasutada [sõnumi jälg](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) leida sõnumeid ja nende vastava sõnumi ID väärtused.
- **Saatja e-posti aadress**: ühe saatja meiliaadress.
- **Adressaadi e-posti aadress**: ühe adressaadi meiliaadress.
- **Teema**: kasutage sõnumi tervet teemat. Otsing ei ole tõstutundlik.

Pärast otsingukriteeriumide sisestamist klõpsake tulemuste filtreerimiseks nuppu Värskenda ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** .  

Cmdlet-käsud abil saate vaadata ja hallata karantiini sõnumeid ja faile on:
- [Kustuta-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksport-Kvarantinemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Hankige-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Eelvaade-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): pange tähele, et see cmdlet-käsk on ainult sõnumeid, mitte PAHAVARA faile ATP SharePoint Online, OneDrive for Business või meeskonnad.
- [Vabastamine-Kvarantinemessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)