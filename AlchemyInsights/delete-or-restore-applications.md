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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014798"
---
# <a name="delete-or-restore-applications"></a>Rakenduste kustutamine või taastamine

**AZURE ad rentniku rakenduse kustutamiseks tehke** järgmist.

1. Valige **AZURE ad portaalis** **Enterprise Applications (Enterprise Applications**). Seejärel otsige üles ja valige rakendus, mille soovite kustutada.
2. Klõpsake vasakpoolse paani jaotises **haldamine** nuppu **Atribuudid**.
3. Valige **Kustuta** ja seejärel valige **Jah** , et kinnitada, et soovite rakenduse Azure AD rentnikult kustutada.

Lisateavet rakenduse kustutamise kohta leiate teemast [Kiirjuhend: rakenduse kustutamine Azure Active Directory (AZURE ad) rentniku kaudu](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

PowerShellis eemaldab cmdlet [-käsk Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) rakenduses Azure Active Directory teatud rakenduse puhverserveri konfiguratsioonid ja saab rakenduse täielikult kustutada, kui see on määratud.

**Kustutatud rakenduse saate taastada** PowerShelli abil. Kui rakendus, mille soovite taastada, on tuvastatud, saate selle taastada, kasutades [AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
