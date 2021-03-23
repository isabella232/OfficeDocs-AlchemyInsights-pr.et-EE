---
title: Azure Active Directory läbimise autentimise konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035539"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a>Azure Active Directory läbimise autentimise konfigureerimine

Siin on mõned juhised, mis aitavad teil konfigureerida läbima autentimise.

- **Azure Active Directory ühenduse häälestamiseks** tehke järgmist. [kasutajate sünkroonimine kataloogiteenuse](https://admin.microsoft.com/AdminPortal/Home) abil aitab teil konfigureerida parooli Hash sünkroonimise või läbitud autentimise. See konfiguratsioon võimaldab kasutajatel logida sisse oma e-posti ja asutusesisese Active Directory (domeenikontroller) sama parooliga.  [Teie kataloogiteenuse kasutajate sünkroonimisel](https://admin.microsoft.com/AdminPortal/Home) kehtib ka Federation sign-in for Active Directory Federation Services (AD FS).

- **Azure ' i funktsioonide häälestamiseks tehke** järgmist. Azure ' i [ad setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) ' i abil saate häälestada Azure Active Directory põhifunktsioonid (nt rühma-põhise Accessi haldus, iseteeninduskeskuse parooli lähtestamine pilveteenuse rakenduste jaoks ja Azure Active Directory rakenduse puhverserveri asutusesisese veebirakenduse avaldamiseks).


