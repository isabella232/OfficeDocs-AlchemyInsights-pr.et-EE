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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994798"
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
> [!NOTE]
> **DomainGUID** on tekst, mis **jääb kohandatud domeeni kohandatud MX-kirjes (nt** domeeni contoso-com mail.protection.outlook.com)-st contoso.com **vasakul.** **InitialDomain** on domeen, mida kasutasite Office 365 **(nt contoso.onmicrosoft.com).**

Lisateavet DNS-i kirjete kohta leiate teemast DNS-i kirjete loomine mis [tahes DNS-hostiteenuse pakkuja Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).