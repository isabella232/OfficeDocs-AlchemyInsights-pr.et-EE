---
title: Lisandmoodulite juurutamine Microsoft 365 rakendused
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031402"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Lisandmoodulite juurutamine Microsoft 365 rakendused

Tsentraliseeritud juurutamine on soovitatav viis Office juurutada oma asutuse kasutajatele ja rühmadele lisandmooduleid. Lisandmoodulite juurutamiseks tehke järgmist.

**Märkus.** Lisandmoodulite installimiseks üksikkasutajana Office lugege teemat Lisandmoodulite vaatamiseks, haldamiseks ja [installimiseks Office programmides.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Samuti veenduge, et Office store'i lisandmoodulite individuaalne hankimine oleks lubatud. Lisateavet leiate teemast Lisandmoodulite allalaadimise keelamine, kui lülitate Office poe välja [(v.a Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

1. Veenduge, et teie keskkond vastaks tsentraliseeritud juurutuse abil lisandmoodulite juurutamise nõuetele. Lisateavet leiate teemast [Nõuded](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Lisandmoodulite **Sätted** avage Microsoft 365 halduskeskus rakenduste  >    >   toomine. 

Märkmed: 

- Integreeritud rakenduste kasutamiseks peab administraatoril olema üldadministraatori või Exchange administraatoriõigused.

- Kui juurutate lisandmooduleid mitmele kasutajale, soovitame teha ülesandeid üksikute kasutajate asemel rühmade abil. Lisateavet leiate teemast Lisandmooduli määramise kaalutlused [kasutajatele ja rühmadele.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Tsentraliseeritud juurutus ei toeta pesastatud rühmade või emarühmadega rühmade kasutajaid. Lisateavet leiate teemast [Kasutaja ja rühma ülesanded.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Veenduge, et Microsoft 365-rakendusehaldusteenus (GUID: "0517ffae-825d-4aff-999e-3f2336b8a20a") oleks sisse logimiseks lubatud. Lisateavet leiate teemast [Rakenduse atribuutide konfigureerimine.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Kui teil on probleeme lisandmoodulite juurutamisel integreeritud rakenduste abil, proovige juurutada [lisandmoodulite abil.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Lisateavet leiate järgmistest teemadest.

[Lisandmoodulite juurutamine halduskeskuses](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Lisandmoodulite haldamine halduskeskuses](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Lisandmoodulite haldamine tsentraliseeritud juurutuse PowerShelli cmdlet-käskude abil](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Avaldage Office lisandmoodulid tsentraliseeritud juurutuse abil Microsoft 365 halduskeskus](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Tõrkeotsing. Kasutaja ei näe lisandmooduleid](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Kasutajate tõrgete tõrkeotsing Office lisandmoodulitega](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)