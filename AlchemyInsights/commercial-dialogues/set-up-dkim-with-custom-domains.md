---
title: DKIM-i häälestamine kohandatud domeenidega
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332303"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM-i häälestamine kohandatud domeenidega

Iga dns-i kohandatud domeeni kohta tuleb avaldada kaks CNAME-kirjet. Selleks kasutage järgmist vormingut.

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Märkus.** **DomainGUID** on tekst, mis **asub kohandatud domeeni kohandatud MX-kirjes vasakul mail.protection.outlook.com .contoso.com.**  **InitialDomain** on domeen, mida kasutasite Office 365 **(nt contoso.onmicrosoft.com).**

LISATEAVET DNS-i kirjete kohta leiate teemast DNS-i kirjete loomine mis [tahes DNS-hostiteenuse pakkuja Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).