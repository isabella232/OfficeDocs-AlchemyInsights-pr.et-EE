---
title: 929 sisendkausta reegleid deflectTransport eeskirjad
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 140cb6e85d0f08393439b023578457998a84dc62
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499586"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>E-posti voolu reeglite (tuntud ka kui transpordireeglid)

- Üldise ülevaate posti voog reeglid: [posti voolu reeglid (transpordireeglid) Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- Setup voolu Meilireeglid: [posti voolu reegel kord Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- Luua, muuta ja kustutada e-posti voolu reeglite: [Halda e-posti voolu reeglite](https://technet.microsoft.com/library/jj657505.aspx)

Saate hallata e-posti voolu reeglite Exchange Online PowerShelli. Lisateabe saamiseks vt [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (luua), [Eemalda-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Komplekt-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (muuta), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (Keela olemasoleva), ja [Luba TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (võimaldada olemasolevate).

E-posti voolu reegel cmdlet-käske: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (loendis Saadaolevad toimingud), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (loendis Saadaolevad tingimused ja erandid), [Ekspordi-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (ekspordi reeglid) ja [ Impordi-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (impordi).
