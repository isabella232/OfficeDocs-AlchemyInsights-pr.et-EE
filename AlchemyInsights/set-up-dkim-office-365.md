---
title: Setup DKIM Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666260"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM Office 365

Täielikud juhised konfigureerimine DKIM kohandatud domeenide Office 365 on [siin](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Iga** kohandatud domeeni, peate looma **kaks** DKIM CNAME kirjeid oma domeeni DNS-i hosting teenus (tavaliselt, domeeni kohtusekretäri). Näiteks contoso.com ja fourthcoffee.com nõuavad nelja DKIM CNAME kirjeid: kaks contoso.com ja kaks fourthcoffee.com.

   DKIM CNAME kirjed **iga** kohandatud domeeni kasutada järgmisi vorminguid:

   - **Hosti nimi**:`selector1._domainkey.<CustomDomain>`

     **Osutab aadressile või väärtusele**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hosti nimi**:`selector2._domainkey.<CustomDomain>`

     **Osutab aadressile või väärtusele**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on kohandatud domeeni kohandatud MX-kirjes vasakul `.mail.protection.outlook.com` olev tekst (nt domeeni contoso.com `contoso-com` puhul). \<InitialDomain\> on domeen, mida kasutasite, kui registreerite Office 365 (nt contoso.onmicrosoft.com).

2. Pärast seda, kui olete loonud oma kohandatud domeenide CNAME-kirjed, täitke järgmised juhised:

   A. [Logige sisse Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) oma töö või kooli kontoga.

   B. Valige ülemise vasakpoolse rakenduse käivitaja ikoon ja valige **admin**.

   C. Alumises vasakus navigeerimise, laiendage **admin** ja valige **Exchange**.

   D. Mine **kaitse** > **DKIM**.

   E. Valige domeen ja seejärel valige **Luba** **Logi sõnumid selle domeeni DKIM allkirjad**. Korrake seda toimingut iga kohandatud domeeni puhul.
