---
title: DKIM setup probleemide lahendamine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717558"
---
# <a name="fix-dkim-setup-issues"></a>DKIM setup probleemide lahendamine

Kui teil tekib probleeme, mis võimaldavad DKIM oma kohandatud domeeni, toimige järgmiselt.

- Enamik DKIM setup probleemid on seotud vale DNS-kirjete. Kontrollige DKIM CNAME kirje (**mitte** TXT kirje) on õigesti vormindatud. Lisateabe saamiseks vaadake seda [teemat](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Pärast seda, kui loote või värskendage oma DKIM DNS-kirjete DNS-i hosting teenus domeeni (tavaliselt, teie domeeni kohtusekretäri), oodake DNS-kirjete paljundada.

- Kui te ei saa luua DKIM DNS-kirjete administreerimiskeskus, saate \<asendada customdomain\> oma kohandatud domeeni (nt contoso.com) ja käivitage see käsk [Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
