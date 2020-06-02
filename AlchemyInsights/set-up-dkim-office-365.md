---
title: Setup DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509380"
---
# <a name="setup-dkim"></a>Setup DKIM

Täielikud juhised konfigureerimine DKIM kohandatud domeenide Microsoft 365 on [siin](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. **Iga** kohandatud domeeni, peate looma **kaks** DKIM CNAME kirjeid oma domeeni DNS-i hosting teenus (tavaliselt, domeeni kohtusekretäri). Näiteks contoso.com ja fourthcoffee.com nõuavad nelja DKIM CNAME kirjeid: kaks contoso.com ja kaks fourthcoffee.com.

   DKIM CNAME kirjed **iga** kohandatud domeeni kasutada järgmisi vorminguid:

   - **Hosti nimi**:`selector1._domainkey.<CustomDomain>`

     **Osutab aadressile või väärtusele**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hosti nimi**:`selector2._domainkey.<CustomDomain>`

     **Osutab aadressile või väärtusele**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>on `.mail.protection.outlook.com` kohandatud domeeni kohandatud MX-kirjes vasakul olev tekst (nt `contoso-com` domeeni contoso.com). \<InitialDomain\>on domeen, mida kasutasite, kui registreerite Microsoft 365 (nt contoso.onmicrosoft.com).

2. Pärast seda, kui olete loonud oma kohandatud domeenide CNAME-kirjed, täitke järgmised juhised:

   A. [logige sisse Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) oma töö või kooli kontoga.

   B. Valige ülemise vasakpoolse rakenduse käivitaja ikoon ja valige **admin**.

   C. Alumises vasakus navigeerimise, laiendage **admin** ja valige **Exchange**.

   D. Mine **kaitse**  >  **DKIM**.

   E. Valige domeen ja seejärel valige **Luba** **Logi sõnumid selle domeeni DKIM allkirjad**. Korrake seda toimingut iga kohandatud domeeni puhul.
