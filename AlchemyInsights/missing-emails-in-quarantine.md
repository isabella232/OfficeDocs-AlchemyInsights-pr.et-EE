---
title: Puuduvad meilid karantiinis
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673710"
---
# <a name="missing-emails-in-quarantine"></a>Puuduvad meilid karantiinis "

Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Turbe & täitmise keskuse avamiseks valige [https://protection.office.com](https://protection.office.com/) . Otse karantiini lehe avamiseks avage [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Saate otsida järgmiste väärtuste järgi.  

- **Sõnumi ID**: sõnumi globaalselt kordumatu identifikaator. Kui valite loendist sõnumi, kuvatakse kuvatavas hüpik paanil **sõnumi ID** väärtus. **Details** Administraatorid saavad sõnumite otsimiseks ja vastavate sõnumi ID-väärtuste otsimiseks kasutada [sõnumi jälgi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) .
- **Saatja**meiliaadress: ühe saatja meiliaadress.
- **Adressaadi meiliaadress**: ühe adressaadi meiliaadress.
- **Teema**: kasutage sõnumi kogu teemat. Otsing pole tõstutundlik.

Kui olete otsingukriteeriumid sisestanud, klõpsake ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** tulemite filtreerimiseks nuppu Värskenda.  

Karantiinis olevate sõnumite ja failide vaatamiseks ja haldamiseks kasutatavad cmdlet-käsud on järgmised.
- [Kustutamine – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Eksport – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Eelvaade – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): pange tähele, et see cmdlet on mõeldud ainult sõnumitele, mitte ründevarale SharePoint Online ' i, OneDrive for Businessi või TEAMsi ATP-St.
- [Väljalase – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)