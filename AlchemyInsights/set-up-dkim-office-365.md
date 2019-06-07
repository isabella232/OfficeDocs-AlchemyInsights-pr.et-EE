---
title: Setup DKIM Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765011"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM Office 365

Täielikud juhised konfigureerimiseks DKIM kohandatud domeenide Office 365 on [siin](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. **Iga** kohandatud domeeni, peate looma **kaks** DKIM CNAME-kirjeid, teie domeeni DNS-i hostimisteenuses (tavaliselt domeeniregistraatori). Nt contoso.com ja fourthcoffee.com nõuavad neli DKIM CNAME-kirjeid: kaks contoso.com ja kaks fourthcoffee.com.

   **Iga** kohandatud domeeni DKIM CNAME-kirjeid kasutada järgmisi vorminguid:

   - **Serveri nimi**:`selector1._domainkey.<CustomDomain>`

     **Aadress või väärtus viitab**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Serveri nimi**:`selector2._domainkey.<CustomDomain>`

     **Aadress või väärtus viitab**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> on tekst vasakul `.mail.protection.outlook.com` MX-kirjes kohandatud kohandatud domeeni (nt `contoso-com` jaoks domeeni contoso.com). \<InitialDomain\> on domeen, kui olete registreerunud Office 365 (nt contoso.onmicrosoft.com).

2. Pärast loomist kohandatud domeenide CNAME-kirjeid, täitke järgmised juhised:

   saanud. [Office 365 sisselogimine](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) töö- või koolikontoga kontoga.

   b. Valige rakenduse käivitaja ikoon ülemises vasakus ja **Admin**.

   c. Vasakus navigation, laiendada **Admin** ja valige **Exchange**.

   d. Mine **kaitse** > **DKIM**.

   e. Valige domeeni ja valige **lubade kasutada programmi** **Logi**sõnumeid selle domeeni DKIM allkirjad. Korrake seda toimingut iga kohandatud domeeni.
