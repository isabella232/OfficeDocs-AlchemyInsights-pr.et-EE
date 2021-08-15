---
title: Karantiinis puuduvad meilisõnumid
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
- "5668"
- "9002625"
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026218"
---
# <a name="missing-emails-in-quarantine"></a>Karantiinis puuduvad meilisõnumid"

Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Turbe- & avamiseks avage [https://protection.office.com](https://protection.office.com/) . Karantiinilehe otse avamiseks avage [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Saate otsida järgmiste väärtuste järgi.  

- **Sõnumi ID:** sõnumi globaalne ainuidentifikaator. Kui valite loendist sõnumi, kuvatakse kuvataval hüpikpaanil **Üksikasjad** väärtus Sõnumi **ID.** Administraatorid saavad [sõnumijälitus abil](/microsoft-365/security/office-365-security/message-trace-scc) otsida sõnumeid ja neile vastavaid sõnumi ID väärtusi.
- **Saatja meiliaadress:** ühe saatja meiliaadress.
- **Adressaadi meiliaadress:** ühe adressaadi meiliaadress.
- **Teema:** kasutage kogu sõnumi teemat. Otsing pole stiotsingutundlik.

Kui olete otsingukriteeriumid sisestanud, klõpsake ![ tulemite ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **filtreerimiseks** nuppu Värskenda.

Cmdlet-käsud, mida kasutate sõnumite ja failide karantiinis kuvamiseks ja haldamiseks, on järgmised.
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Ekspordi-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Pange tähele, et see cmdlet-käsk on ainult sõnumite, mitte Microsoft Defenderi ründevarafailide Office 365 jaoks SharePoint Online'i, OneDrive for Business või Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)