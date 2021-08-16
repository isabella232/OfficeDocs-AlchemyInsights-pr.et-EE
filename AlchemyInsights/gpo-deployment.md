---
title: GPO juurutamine
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
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067836"
---
# <a name="gpo-deployment"></a>GPO juurutamine

Sätted (Azure AD DS) kasutaja- ja arvutiobjektide Azure Active Directory hallatakse sageli rühmapoliitika objektide (GPO) abil. Azure AD DS sisaldab sisseehitatud GPO-sid AADDC kasutajate ja AADDC arvutite ümbriste jaoks. Saate kohandada neid sisseehitatud GPO-sid, et konfigureerida rühmapoliitika vastavalt oma keskkonna jaoks vajalikule. Azure AD DC administraatorite rühma liikmetel on Azure AD DS-i domeenis rühmapoliitika haldusõigused ning nad saavad luua ka kohandatud GPO-sid ja organisatsiooniüksusi (OU-sid). Lisateavet rühmapoliitika ja selle töö kohta leiate teemast [Rühmapoliitika ülevaade](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Hübriidkeskkonnas ei sünkroonita asutusesiseseS AD DS-keskkonnas konfigureeritud rühmapoliitikaid Azure AD DS-iga. Azure AD DS-i kasutajate või arvutite konfiguratsioonisätete määratlemiseks redigeerige ühte vaike-GPO-dest või looge kohandatud GPO.

Selles artiklis [rühmapoliitika haldamine selgitatakse,](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) kuidas installida rühmapoliitika haldustööriistu, kuidas redigeerida sisseehitatud GPO-sid ja kuidas luua kohandatud GPO-sid.
