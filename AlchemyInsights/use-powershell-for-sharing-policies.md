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
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998462"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShelli kasutamine ühiskasutuspoliitika ja organisatsiooniseoste jaoks


Organisatsiooniseoste jaoks tutvuge üksikasjaliku süntaksi- ja parameetriteabega: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  JA  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Ühiskasutuspoliitika loomiseks kasutage funktsiooni [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Et  [rakendada ühiskasutuspoliitikat postkastile või kasutajale](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  peate kasutama koos vastloodud poliitikaga  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinatsiooni. Et  [muuta, keelata või eemaldada ühiskasutuspoliitikat](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  peate kasutama funktsioone  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Selle teema täielikuks mõistmiseks lugege:**

[Ühiskasutus Exchange Online‘is](https://docs.microsoft.com/exchange/sharing/sharing)