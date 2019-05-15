---
title: Ei saa kustutada OneDrive'i või SharePointi üksuste
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057700"
---
# <a name="unable-to-delete-items"></a>Ei saa üksusi kustutada

Üksuste kustutamine probleeme?

- Alati veenduge, et teil on [vastavad õigused](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) kustutada üksuse või [saidikogumi administraator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) katse üksuse eemaldada.

- Tagada, et üksusel ei ole [säilituspoliitika](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup.

- Tagada, et kaup ei ole mõnele teisele kasutajale [välja möllitud](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) .

- Administraatorid saavad kasutada [SharePoint ja tavasid](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) mis sisaldab Raamatukogu PowerShelli käsud, mille abil saab keerulisi juhtimise toiminguid nagu sundida kangekaelne üksuste kustutamine. 
- [PNP faili eemaldamiseks](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP kausta eemaldamine](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP loendiüksuse eemaldada](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Eemalda PNP loend](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Eemalda PNP väli (veerg)](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)