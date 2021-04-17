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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831730"
---
# <a name="missing-emails-in-quarantine"></a>Karantiinis puuduvad meilisõnumid"

Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Turbe- & avamiseks avage [https://protection.office.com](https://protection.office.com/) . Karantiinilehe otse avamiseks avage [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Saate otsida järgmiste väärtuste järgi.  

- **Sõnumi ID:** sõnumi globaalne ainuidentifikaator. Kui valite loendist sõnumi, kuvatakse kuvataval hüpikpaanil **Üksikasjad** väärtus Sõnumi **ID.** Administraatorid saavad [sõnumijälitus abil](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) otsida sõnumeid ja neile vastavaid sõnumi ID väärtusi.
- **Saatja meiliaadress:** ühe saatja meiliaadress.
- **Adressaadi meiliaadress:** ühe adressaadi meiliaadress.
- **Teema:** kasutage kogu sõnumi teemat. Otsing pole stiotsingutundlik.

Kui olete otsingukriteeriumid sisestanud, klõpsake ![ tulemite ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **filtreerimiseks** nuppu Värskenda.  

Cmdlet-käsud, mida kasutate sõnumite ja failide karantiinis kuvamiseks ja haldamiseks, on järgmised.
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Ekspordi-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Pange tähele, et see cmdlet-käsk on ainult sõnumite, mitte ründevarafailide jaoks, mis on pärit SharePoint Online'i, OneDrive for Businessi või Teamsi ATP-st.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)