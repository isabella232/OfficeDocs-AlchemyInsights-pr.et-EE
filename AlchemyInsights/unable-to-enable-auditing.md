---
title: 2419-ei saa lubada-auditeerimine
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510424"
---
# <a name="unable-to-enable-unified-auditing"></a>Ühtset auditeerimist ei saa lubada

Kui proovite lubada oma organisatsiooni ühendatud auditeerimine, võidakse kuvada tõrketeade, mis sarnaneb järgmisega:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Selle probleemi lahendamiseks toimige järgmiselt.

1. [Ühendust Exchange Online PowerShelli](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Käivitage järgmine cmdlet-käsk:

   ```
   Enable-OrganizationCustomization
   ```

3. Oodake 60 minutit eelmise sätte jõustumiseks.

4. Käivitage järgmine käsk Exchange Online PowerShelli:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lisateabe saamiseks lugege järgmisi artikleid:

- [Ühendamine Exchange Online PowerShelli abil mitme teguriga autentimine](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Auditilogi otsingu sisse-või väljalülitamine](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
