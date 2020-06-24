---
title: PowerShelli kasutamine poliitikate ja organisatsiooniseoste ühiskasutuseks
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862056"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShelli kasutamine poliitikate ja organisatsiooniseoste ühiskasutuseks


Organisatsiooni seoste puhul vaadake üksikasjalikku süntaksi ja parameetri teavet: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ja [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Ühiskasutuspoliitika loomiseks kasuta [teemat New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). [Ühiskasutuse poliitika rakendamiseks postkastile või kasutajale](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) peate kasutama vastloodud poliitikaga [set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ja [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) kombinatsiooni. Ühiskasutuse [poliitika muutmiseks, keelamiseks või eemaldamiseks](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) peate kasutama [valikut Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ja [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Täielikuks mõistmiseks selle teema palun lugeda:**

[Ühiskasutus Exchange Online'is](https://docs.microsoft.com/exchange/sharing/sharing)