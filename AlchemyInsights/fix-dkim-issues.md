---
title: DKIM-i häälestusprobleemide lahendamine
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945927"
---
# <a name="fix-dkim-setup-issues"></a>DKIM-i häälestusprobleemide lahendamine

Kui teil on probleeme DKIM-i lubamisega oma kohandatud domeeni jaoks, tehke järgmist.

- Enamik DKIM-i häälestusprobleeme on seotud valede DNS-i kirjetega. Veenduge, et DKIM-i **CNAME-kirje** (mitte TXT-kirje) oleks õigesti vormindatud. Lisateavet leiate teemast [.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Pärast DKIM-i DNS-i kirjete lisamist või värskendamist domeeni DNS-hostiteenuses (tavaliselt teie domeeniregistraator) oodake, kuni DNS-i kirjed levivad.

- Kui te ei saa halduskeskuses DKIM-i DNS-i kirjeid luua, saate asendada kohandatud domeeniga (nt contoso.com) ja käivitada selle käsu \<CustomDomain\> [Exchange Online PowerShellis.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
