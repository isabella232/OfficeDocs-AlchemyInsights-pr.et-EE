---
title: Rakenduse Intune Win32 juurutamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461794"
---
# <a name="intune-win32-app-deployment"></a>Rakenduse Intune Win32 juurutamine

Microsoft Intune võimaldab Win32 rakendused, sealhulgas, kuid mitte ainult MSI ja. EXE tuleb juurutada Windows 10 seadmetes. Kasutatava juurutuse mehhanismi jaoks on vaja Intune Managementi laiendit (IME), et see oleks TARGETi seadmes olemas. IME installitakse automaatselt, kui see on suunatud PowerShelli skriptile või Win32-rakenduse juurutusele kasutajale/seadmele.

Olemas on ka komplekt eeltingimustest, mis peavad olema täidetud, et juurutada Win32 rakendusi, mis sisaldavad järgmist:

- Toetatud platvormid: Windows 10 versioon 1607 või uuem versioon (Enterprise, Pro ja Educationi versioonid).
- Toetatud arhitektuur: x86 ja x64.
- Seadme haldus: AAD liitunud ja automaatselt registreerunud (sh hübriid-Domeen liidetud ja rühmapoliitika automaatselt registreerunud).
- Rakenduse paketi vorming:. [Microsoft Win32 sisu prep tööriist](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)on koostanud **intunewin** -failid.
- Piirangud
    - Maksimaalne suurus: 8GB.
    - Toetuseta arhitektuur: relvad.

Vaadake üle doc "[Lisa, määra ja jälgige Microsoft Intune ' is Win32 rakendust](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)".

Windowsi rakenduste juurutuse tõrkeotsingu üksikasju (sh Win32 rakendusi) saab vaadata järgmistes dokumentides.

- [Rakenduse installimise probleemide tõrkeotsing](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 rakenduste tõrkeotsing](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)