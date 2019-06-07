---
title: DKIM installiprobleemide lahendamiseks
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764999"
---
# <a name="fix-dkim-setup-issues"></a>DKIM installiprobleemide lahendamiseks

Kui teil tekib küsimusi, mis võimaldavad DKIM oma kohandatud domeeni, tehke järgmist:

- Enamik DKIM installiprobleemide on seotud vale DNS-kirjeid. Kontrollida (**ole** TXT-kirje) DKIM CNAME-kirje on õigesti vormindatud. Lisateavet vt selle [teema](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Pärast loomist või värskendada oma DKIM DNS-kirjeid DNS-i hostimisteenuses domeeni (tavaliselt oma domeeniregistraatori), oodake, kuni DNS-kirjete propageerida.

- Kui te ei saa luua DKIM DNS kirjed administreerimiskeskuses, saate asendada \<CustomDomain\> kohandatud domeeni (nt contoso.com) ja piisavaid [Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)PowerShelli: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
