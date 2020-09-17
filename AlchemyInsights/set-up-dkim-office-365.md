---
title: DKIM häälestamine
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808703"
---
# <a name="setup-dkim"></a>DKIM häälestamine

Microsoft 365 kohandatud domeenide DKIM konfigureerimise terviklikud juhised on [siin](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. **Iga** kohandatud domeeni jaoks peate looma **kaks** DKIM CNAME-kirjet oma domeeni DNS-i hostimise teenuses (tavaliselt domeeni registripidaja). Näiteks contoso.com ja fourthcoffee.com nõuavad nelja DKIM CNAME-kirjet: kaks contoso.com ja kaks fourthcoffee.com jaoks.

   **Iga** kohandatud domeeni DKIM CNAME-kirjed kasutavad järgmisi vorminguid.

   - **Hosti nimi**: `selector1._domainkey.<CustomDomain>`

     Osutage **aadressile või väärtusele**.`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hosti nimi**: `selector2._domainkey.<CustomDomain>`

     Osutage **aadressile või väärtusele**.`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on `.mail.protection.outlook.com` kohandatud domeeni kohandatud MX-kirjest vasakul asuv tekst (nt `contoso-com` domeeni contoso.com). \<InitialDomain\> on domeen, mida kasutasite Microsoft 365 kasutajaks registreerumisel (nt contoso.onmicrosoft.com).

2. Kui olete oma kohandatud domeenide jaoks loonud CNAME-kirjed, tehke järgmised juhised.

   loomine. [logige sisse rakendusse Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) oma töökoha või kooli kontoga.

   b. Valige vasakus ülanurgas rakenduse käivitaja ikoon ja valige **administraator**.

   c. Laiendage vasakus allnurgas nuppu **administraator** ja valige **Exchange**.

   d. Avage **kaitse**  >  **DKIM**.

   e. Valige domeen ja seejärel valige **DKIM allkirjaga selle domeeni jaoks sõnumite allkirjastamise** **lubamine** . Korrake seda toimingut iga kohandatud domeeni korral.
