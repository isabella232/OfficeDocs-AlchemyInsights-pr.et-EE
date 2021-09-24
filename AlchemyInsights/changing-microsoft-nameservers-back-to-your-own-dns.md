---
title: Microsofti nimeserveritelt tagasi oma DNS-i kirjete haldamisele üleminek
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506384"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Microsofti nimeserveritelt tagasi oma DNS-i kirjete haldamisele üleminek

Olete varem muutnud oma NS-kirjeid osutama Microsoftile (ns1.bdm.microsoftonline.com), kuid olete nüüd otsustanud hallata oma DNS-i kirjeid.

Muutke oma domeeniregistraatori veebisaidil nimeserver tagasi oma registraatoriks või eelmiseks sätteks. Kui te pole DNS-iga tuttav, pöörduge domeeniregistraatori poole. Pange tähele, et nimeserveri muudatuste levimiseks võib aega võtta kuni 48 tundi. 

1. Avage Microsoft 365 haldusportaalis **Sätted** Domeenid , märkige domeeni kõrval ruut  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)ja valige **Halda DNS-i**. 

2. Valige viisardis **Add your own DNS records (Lisa oma DNS-i kirjed)** ja täitke viisard. See muudab teie DNS-i hallata ja seejärel saate lisada kohandatud DNS-i kirjed, mis on vajalikud teie valitud teenuste toetamiseks.

Kui muutsid nimeserverikirjed Microsoftiks ja teil on veebisait, saate nimeserverite tagasi muutmise asemel lisada veebisaidile DNS-i kirjed. Lisateavet leiate teemast [Dns-i kirjete värskendamine, et säilitada oma veebisait praeguse majutusteenuse pakkuja juures.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


