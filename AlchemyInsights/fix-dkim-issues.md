---
title: DKIM lahendamise probleemide lahendamine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744946"
---
# <a name="fix-dkim-setup-issues"></a>DKIM lahendamise probleemide lahendamine

Kui teil ilmnevad probleemid, mis võimaldavad DKIM teie kohandatud domeeni jaoks, tehke järgmist.

- Enamik DKIM installimisega seotud probleemidest on seotud valede DNS-i kirjetega. Veenduge, et DKIM CNAME-kirje (**mitte** TXT-kirje) oleks õigesti vormindatud. Lisateavet leiate sellest [teemast](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Pärast seda, kui olete oma domeeni DNS-i DKIM loonud või värskendanud DNS-i kirjeid (tavaliselt teie domeeni registripidaja), oodake, kuni DNS-i kirjed on paljundatud.

- Kui te ei saa DKIM DNS-i kirjeid luua, saate asendada \<CustomDomain\> kohandatud domeeniga (nt contoso.com) ja käivitada selle käsu [Exchange Online PowerShellis](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
