---
title: 2419-ei saa-to-enable-audit
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767595"
---
# <a name="unable-to-enable-unified-auditing"></a>Ühtset auditit ei saa lubada

Kui proovite lubada oma asutuse jaoks ühendatud auditit, võidakse kuvada tõrketeade, mis sarnaneb järgmisega:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Probleemi lahendamiseks tehke järgmist.

1. [Ühenduse loomine Exchange Online PowerShelliga](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Käivitage järgmine cmdlet-käsk:

   ```
   Enable-OrganizationCustomization
   ```

3. Oodake, kuni eelmise säte jõustub 60 minutit.

4. Exchange Online PowerShellis käivitage järgmine käsk:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisateavet leiate järgmistest artiklitest.

- [Exchange Online PowerShelliga ühenduse loomine mitme teguri autentimise abil](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Auditilogi otsingu sisse-või väljalülitamine](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
