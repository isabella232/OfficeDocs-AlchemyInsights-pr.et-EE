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
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329658"
---
# <a name="missing-emails-in-quarantine"></a>Karantiinis puuduvad meilisõnumid

Administraatorid saavad [neid sõnumeid vaadata, vabastada või kustutada](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Avage Microsoft 365 Defender portaalis <https://security.microsoft.com> Läbivaatus karantiini  \> . Või otse karantiini lehele **minemiseks** kasutage funktsiooni <https://security.microsoft.com/quarantine> .  

Lisateavet nende otsingu-/filtriväärtuste kohta, mida saate kasutada, leiate teemast Karantiinis sõnumite [ja failide haldamine EOP administraatorina.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Cmdlet-käsud, mida kasutate sõnumite ja failide karantiinis kuvamiseks ja haldamiseks, on järgmised.

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Ekspordi-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Pange tähele, et see cmdlet-käsk on ainult sõnumite jaoks, mitte seif-, SharePoint, OneDrive või Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
