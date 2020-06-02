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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506770"
---
# <a name="fix-dkim-setup-issues"></a>DKIM setup probleemide lahendamine

Kui teil tekib probleeme, mis võimaldavad DKIM oma kohandatud domeeni, toimige järgmiselt.

- Enamik DKIM setup probleemid on seotud vale DNS-kirjete. Kontrollige DKIM CNAME kirje (**mitte** TXT kirje) on õigesti vormindatud. Lisateabe saamiseks vaadake seda [teemat](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Pärast seda, kui loote või värskendage oma DKIM DNS-kirjete DNS-i hosting teenus domeeni (tavaliselt, teie domeeni kohtusekretäri), oodake DNS-kirjete paljundada.

- Kui te ei saa luua DKIM DNS-kirjete administreerimiskeskus, saate asendada \<CustomDomain\> oma kohandatud domeeni (nt contoso.com) ja käivitage see käsk [Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
