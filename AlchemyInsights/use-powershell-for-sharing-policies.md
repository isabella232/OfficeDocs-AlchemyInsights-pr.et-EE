---
title: PowerShelli kasutamine ühiskasutuspoliitika ja organisatsiooniseoste jaoks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: et-EE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709462"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShelli kasutamine ühiskasutuspoliitika ja organisatsiooniseoste jaoks


Organisatsiooniseoste jaoks tutvuge üksikasjaliku süntaksi- ja parameetriteabega: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  JA  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Ühiskasutuspoliitika loomiseks kasutage funktsiooni [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Et  [rakendada ühiskasutuspoliitikat postkastile või kasutajale](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  peate kasutama koos vastloodud poliitikaga  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinatsiooni. Et  [muuta, keelata või eemaldada ühiskasutuspoliitikat](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  peate kasutama funktsioone  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Selle teema täielikuks mõistmiseks lugege:**

[Ühiskasutus Exchange Online‘is](https://docs.microsoft.com/exchange/sharing/sharing)