---
title: Blokeeri allalaadimise lingid
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357630"
---
# <a name="block-download-on-sharing-links"></a>Blokeeri allalaadimise lingid

**Blokeeri allalaadimine** on saadaval ainult Office ' i dokumentidele mõeldud **linkide kuvamiseks** . Selle suvandi valimisel ei näe inimesed, kes pääsevad failile juurde teie loodud lingi kaudu, suvandeid alla laadida, printida ega kopeerida.

Administraatorid saavad kontrollida, kas "Block alla" säte kuvatakse ainult Office ' i failid või mitte, muutes `BlockDownloadLinksFileType` sätet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) või [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShelli cmdlet-käsud.
