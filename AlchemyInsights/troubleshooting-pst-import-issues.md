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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059811"
---
# <a name="troubleshooting-pst-import-issues"></a>PST importimise probleemide tõrkeotsing

- Kui impordite Outlooki klientrakenduses endas, lugege teemat Outlooki [PST-faili importimisega seotud probleemide lahendamine.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Kui kasutate imporditeenust ja see on kinni jäänud, võtke arvesse, et iga PST-fail, mille azure'i salvestusruumi üles laadite, ei tohiks olla suurem kui 20 GB. PST-failid, mille maht on suurem kui 20 GB, võivad mõjutada PST-impordiprotsessi jõudlust. Lisateavet kinniste tööde tõrkeotsingu kohta leiate teemast [PST-imporditöid mõjutavad probleemid.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Kui soovite kontrollida kindla imporditöö olekut, kasutage funktsiooni [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Imporditeenuse kohta leiate lisateavet teemast [Ettevõtte PST-failide importimise ülevaade.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
