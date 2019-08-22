---
title: Määrata 0x8004de40 viga OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525055"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Määrata 0x8004de40 viga OneDrive

Kui saate tõrketeate 0x8004de40 OneDrive:

- Kui teie Acitve Directory domeeni mõjutatud arvuti taaskäivitama.
- Kui reboot ei lahenda probleemi, unjoin ja ühineks Azure AD seadmesse. 

**Märkus**: te peate olema ettevõtte võrgus nende teostamisel. Ei täida järgmiselt, kui te ei ole võimalik luua ühendus oma ettevõtte infrastruktuuri (näiteks reisides). 

- Avage administraatoriõigustes Käsuviip. 
- Avage administraatoriõigustes Käsuviip, kliki - **Start**, paremklõpsake **käsku Käsuviip**ja seejärel klõpsake käsku **Käivita administraatorina**.
- Tüüp *dsregcmd /leave* ja vajutage **Enter**.
- Kui kõrvaklapid *dsregcmd /join* tüüp ja vajutage **Enter**.
- Kui valmis, sulgege selle Käsuviip.
- Taaskäivitage arvuti ja logige OneDrive'i.