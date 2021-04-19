---
title: PowerShelli kasutamine ühiskasutuspoliitika ja organisatsiooniseoste jaoks
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826051"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShelli kasutamine ühiskasutuspoliitika ja organisatsiooniseoste jaoks


Organisatsiooniseoste jaoks tutvuge üksikasjaliku süntaksi- ja parameetriteabega: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  JA  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Ühiskasutuspoliitika loomiseks kasutage funktsiooni [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Et  [rakendada ühiskasutuspoliitikat postkastile või kasutajale](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  peate kasutama koos vastloodud poliitikaga  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinatsiooni. Et  [muuta, keelata või eemaldada ühiskasutuspoliitikat](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  peate kasutama funktsioone  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Selle teema täielikuks mõistmiseks lugege:**

[Ühiskasutus Exchange Online‘is](https://docs.microsoft.com/exchange/sharing/sharing)