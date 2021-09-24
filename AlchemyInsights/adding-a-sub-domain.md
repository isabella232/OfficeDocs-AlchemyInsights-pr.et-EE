---
title: Alamdomeeni lisamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506325"
---
# <a name="adding-a-sub-domain"></a>Alamdomeeni lisamine

Alamdomeenid saab lisada emadomeeniga samale või muule rentnikule. Mõlemal juhul peate haldama oma DNS-i sätteid oma registraatori veebisaidil. Kui olete NS-kirjetega oma DNS-i sätteid haldanud Microsoftil või kui ostsite domeeni Microsoftilt, ei saa alamdomeene lisada ilma seda esmalt muutmata.

Lisage esmalt emadomeen ja seejärel lisage alamdomeen. Kui alamdomeen on samas rentnikus, pole täiendavat kontrollimist vaja. Kui lisate alamdomeeni eraldi rentnikule, on dns-i txt-kirje enne valitud teenuste jaoks domeeni ja täiendavate DNS-i kirjete lisamist omanike kinnitamiseks nõutav.

- Domeeni või alamdomeeni lisamiseks järgige [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)domeeni lisamise viisardit või lisage domeen või alamdomeen käsitsi, avamiseks valige   >  **Domeenide**  >  **lisamise domeeni seadmine**.

Vajaduse korral:

- Olemasoleva domeeni DNS-i sätteid haldav kasutaja muutmiseks avage **Sätted** Domains (Domeenid), märkige domeeni kõrval ruut ja  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)seejärel valige **Halda DNS-i**. Valige viisardis **Add your own DNS records (Lisa oma DNS-i kirjed)** ja täitke viisard.
- Microsofti ostetud domeenile alamdomeenide lisamiseks kandke esmalt domeen üle teisele registraatorile ja seejärel tehke ülaltoodud muudatus, et hallata oma DNS-i kirjeid. Juhised leiate teemast [Domeeni üleviimine Microsoftilt teisele hostile.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Kui teile kuvatakse tõrketeade selle kohta, et teie domeeni kasutavad juba teised teie ettevõtte liikmed või inimesed, peate enne domeeni kasutamist selle mittehallatud konto üle võtma. Juhised leiate teemast [Mittehallatud kataloogi](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)üle Azure Active Directory.
