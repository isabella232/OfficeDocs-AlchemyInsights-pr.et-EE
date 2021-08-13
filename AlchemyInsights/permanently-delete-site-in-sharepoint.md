---
title: Saidi jäädavalt kustutamine SharePointis
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944307"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Saidi jäädavalt kustutamine SharePointis

Kustutatud saidi URL-i uuesti kasutamiseks (saidi taasloomiseks) või saidi jäädavalt kustutamiseks, kuna see pole enam kasutusel, saate kasutada uue SharePointi halduskeskuse suvandit **Kustuta jäädavalt**. 

1. Avage [uue SharePointi halduskeskuse kustutatud saitide leht](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) ja logige sisse kontoga, millel on teie organisatsiooni administraatoriõigused. 

2. Valige vasakpoolses veerus sait. 

3. Klõpsake valikut **Kustuta lõplikult**. 

**Märkus**: rühmadega seotud saite ei saa uues SharePointi halduskeskuses jäädavalt kustutada. Selle asemel tuleb kasutada atribuuti [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Lisateavet vaadake teemast [Saidi jäädavalt kustutamine](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
