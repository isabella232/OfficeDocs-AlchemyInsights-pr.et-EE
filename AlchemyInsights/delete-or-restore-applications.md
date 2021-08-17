---
title: Rakenduste kustutamine või taastamine
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102567"
---
# <a name="delete-or-restore-applications"></a>Rakenduste kustutamine või taastamine

**Rakenduse kustutamiseks Azure AD rentnikust:**

1. Valige **Azure AD portaalis** **Enterprise'i rakendused**. Seejärel otsige üles ja valige rakendus, mille soovite kustutada.
2. Valige **vasakpoolsel** paanil jaotises Haldamine nupp **Atribuudid**.
3. Valige **Kustuta** ja seejärel valige **Jah,** et kinnitada, et soovite rakenduse Azure AD rentnikust kustutada.

Lisateavet rakenduse kustutamise kohta leiate teemast Quickstart: Rakenduse kustutamine Azure Active Directory [(Azure AD) rentnikust.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

PowerShellis eemaldab [cmdlet-käsk Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) rakenduse puhverserveri konfiguratsioonid konkreetsest rakendusest Azure Active Directory ja saate rakenduse täielikult kustutada, kui see on määratud.

Kustutatud rakenduse **saate taastada** PowerShelli abil. Kui taastatav rakendus on tuvastatud, saate selle Taastada [AzureADDeletedApplicationi abil.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
