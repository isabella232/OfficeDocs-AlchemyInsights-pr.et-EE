---
title: Rühmapoliitika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256714"
---
# <a name="group-policy"></a>Rühmapoliitika

Azure Active Directory Domain Services (Azure AD DS) kasutajate ja arvuti objektide sätteid hallatakse sageli rühmapoliitika objektide (GPO) abil. Azure AD DS sisaldab sisseehitatud lubatu AADDC kasutajate ja AADDC arvutite jaoks. Teie keskkonna jaoks vajaliku rühmapoliitika konfigureerimiseks saate kohandada neid sisseehitatud lubatu. Azure AD DC administraatorite rühma liikmetel on Azure AD DS-i domeenis rühmapoliitika halduse privileegid ning saate luua ka kohandatud GPO-d ja korralduslikke üksusi. Lisateavet rühmapoliitika ja selle töötamise kohta leiate teemast [rühmapoliitika ülevaade](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hübriid-keskkonnas ei sünkroonita kohapealses AD DS-keskkonnas konfigureeritud rühmapoliitika Azure AD DS-iga. Azure AD DS-is kasutajate või arvutite jaoks konfiguratsiooniseadete määratlemiseks redigeerige mõnda vaike-lubatu või looge kohandatud GPO.

See artikkel [rühmapoliitika haldamine](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näitab teile, kuidas installida rühmapoliitika juhtimise vahendeid, kuidas ton redigeerida sisseehitatud lubatu ja kuidas luua kohandatud lubatu.



