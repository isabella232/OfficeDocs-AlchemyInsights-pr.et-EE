---
title: 2419-ei saa-et-luba-auditeerimine
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065629"
---
# <a name="unable-to-enable-unified-auditing"></a>Ei saa sisse lülitada ühtse auditeerimise

Kui proovite lubada teie Office 365 organisatsiooni ühtse auditeerimise, te saate tõrketeate, mis on sarnane järgmisega:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Probleemi lahendamiseks toimige järgmiselt.

1. [Exchange Online PowerShelli ühendamine](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Käivitage järgmine cmdlet-käsk:

   ```
   Enable-OrganizationCustomization
   ```

3. Oodake, kuni 60 minutit eelmise sätte jõustamiseks.

4. Exchange Online PowerShelli käivitage järgmine käsk:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisateabe saamiseks lugege järgmisi artikleid:

- [Exchange Online PowerShelli mitmefaktorilist autentimist kasutades ühenduse loomiseks](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 auditi logifaili Otsi sisse- või väljalülitamine](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
