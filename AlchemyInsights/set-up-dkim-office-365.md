---
title: DKIM-i häälestamine
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108552"
---
# <a name="setup-dkim"></a>DKIM-i häälestamine

Siin on täielikud juhised DKIM-i konfigureerimiseks Microsoft 365 [domeenide jaoks.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Iga **kohandatud** domeeni jaoks peate oma domeeni DNS-hostiteenuses (tavaliselt domeeniregistraatoris) looma kaks DKIM-I CNAME-kirjet.  Näiteks nõuavad contoso.com ja fourthcoffee.com nelja DKIM-i CNAME-kirjet: kaks contoso.com ja kaks fourthcoffee.com.

   Iga kohandatud domeeni DKIM-i **CNAME-kirjed** kasutavad järgmisi vorminguid.

   - **Hosti nimi:**`selector1._domainkey.<CustomDomain>`

     **Osutab aadressile või väärtusele:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hosti nimi:**`selector2._domainkey.<CustomDomain>`

     **Osutab aadressile või väärtusele:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on kohandatud domeeni kohandatud MX-kirjest vasakul (nt domeeninimi) vasakul `.mail.protection.outlook.com` `contoso-com` contoso.com. \<InitialDomain\>on domeen, mida kasutasite kasutajaks registreerumisel Microsoft 365 (nt contoso.onmicrosoft.com).

2. Pärast kohandatud domeenide jaoks CNAME-kirjete loomist täitke järgmised juhised.

   a. [logige sisse Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) töö- või koolikontoga.

   b. Valige vasakus ülanurgas rakendusekäiviti ikoon ja valige **Administraator**.

   c. Laiendage vasakpoolsel allnavigeerimispaanil valikut **Administraator** ja **valige Exchange**.

   d. Avage kaitse  >  **DKIM**.

   e. Valige domeen ja seejärel valige käsk **Luba selle** domeeni jaoks sõnumite **signatuur DKIM-signatuuridega.** Korrake seda toimingut iga kohandatud domeeni puhul.
