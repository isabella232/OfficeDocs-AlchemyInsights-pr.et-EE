---
title: Uute OME-võimaluste jaoks IRM-i konfiguratsiooni testimine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812433"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Uute OME-võimaluste jaoks IRM-i konfiguratsiooni testimine

Veendumaks, Microsoft 365 rentnik on konfigureeritud kasutama uusi OME võimalusi, käivitage [PowerShelliga ühenduse Exchange Online cmdlet-käsud.](/powershell/exchange/exchange-online-powershell)


1. Kontrollige rentniku IRM-i konfiguratsiooni, käivitades `Get-IRMConfiguration` . Veenduge, et nende väärtuste väärtuseks oleks **seatud Tõene.**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Käivitage domeeni, saatja aadressi ja adressaadi `Test-IRMConfiguration` kasutamine. Kui test ei läbi, uurige oma IRM-i konfiguratsiooni.

Lisateavet IRM-i konfiguratsiooni kontrollimise kohta leiate teemast Uue [OME konfiguratsiooni kontrollimine Exchange Online PowerShellis.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)