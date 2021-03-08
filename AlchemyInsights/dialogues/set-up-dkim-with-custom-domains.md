---
title: DKIM häälestamine kohandatud domeenide abil
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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524268"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM häälestamine kohandatud domeenide abil

Iga DNS-i kohandatud domeeni jaoks peate avaldama kaks CNAME-kirjet. Selleks kasutage järgmist vormingut.

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** on kohandatud domeeni kohandatud MX-kirjes olevast tekstist Left of **. mail.Protection.Outlook.com** (nt contoso-com domeeni **contoso.com** jaoks). **InitialDomain** on domeen, mida kasutasite Office 365 kasutajaks registreerumisel (nt **contoso.onmicrosoft.com**).

Lisateavet DNS-i kirjete kohta leiate teemast [DNS-i kirjete loomine veebisaidil Office 365 DNS-i majutusteenuse pakkuja](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).