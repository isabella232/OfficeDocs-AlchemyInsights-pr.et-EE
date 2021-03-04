---
title: GPO juurutus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427256"
---
# <a name="gpo-deployment"></a>GPO juurutus

Azure Active Directory Domain Services (Azure AD DS) kasutajate ja arvuti objektide sätteid hallatakse sageli rühmapoliitika objektide (GPO) abil. Azure AD DS sisaldab sisseehitatud lubatu AADDC kasutajate ja AADDC arvutite jaoks. Teie keskkonna jaoks vajaliku rühmapoliitika konfigureerimiseks saate kohandada neid sisseehitatud lubatu. Azure AD DC administraatorite rühma liikmetel on Azure AD DS-i domeenis rühmapoliitika halduse privileegid ning saate luua ka kohandatud GPO-d ja korralduslikke üksusi. Lisateavet rühmapoliitika ja selle töötamise kohta leiate teemast [rühmapoliitika ülevaade](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hübriid-keskkonnas ei sünkroonita kohapealses AD DS-keskkonnas konfigureeritud rühmapoliitika Azure AD DS-iga. Azure AD DS-is kasutajate või arvutite jaoks konfiguratsiooniseadete määratlemiseks redigeerige mõnda vaike-lubatu või looge kohandatud GPO.

See artikkel [rühmapoliitika haldamine](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näitab teile, kuidas installida rühmapoliitika juhtimise vahendeid, kuidas ton redigeerida sisseehitatud lubatu ja kuidas luua kohandatud lubatu.
