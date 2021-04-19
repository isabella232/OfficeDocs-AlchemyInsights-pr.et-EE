---
title: PST importimise probleemide tõrkeotsing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826159"
---
# <a name="troubleshooting-pst-import-issues"></a>PST importimise probleemide tõrkeotsing

- Kui impordite Outlooki klientrakenduses endas, vaadake teemat [Outlooki PST-faili importimise probleemide tõrkeotsing](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Kui kasutate imporditeenust ja see on kinni jäänud, pange tähele, et iga Azure’i talletuskohta üleslaaditav PST-fail ei tohiks olla suurem kui 20 GB. Suuremad kui 20 GB PST-failid võivad mõjutada PST importimise toimingut.

- Kui soovite konkreetse importimise toimingu olekut kontrollida, saate kasutada käsku [Get-MailboxImportRequest -paketi nimi](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Importimisteenuse kõiki detaile vaadake teematst [Organisatsiooni PST-failid importimise ülevaade](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
