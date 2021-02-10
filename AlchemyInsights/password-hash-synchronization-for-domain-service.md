---
title: Domeeni teenuse parooli Hash sünkroonimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177416"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Domeeni teenuse parooli Hash sünkroonimine

**Kui teie Azure AD DS-i eksemplar palub teil parooli räsi sünkroonimise lubada**

Ilmneb stsenaarium, kus töötab hübriid-keskkond, kus kasutajad sünkroonivad kohapealset Azure Active Directory Domain Services (AD DS) keskkonda. See stsenaarium ilmneb hoolimata sellest, et teil on kohapealne AD DS-i Azure AD rentniku jaoks parooli räsi sünkroonimine.

**Põhjustada**

See juhtub, sest Azure AD Connect vaikimisi ei sünkroonita pärand uus tehnoloogia LAN Manageri (NTLM) ja Kerberose parool hashes, mis on vajalik Azure AD DS.

**Ajutine lahendus** 

Peate konfigureerima Azure AD Connecti, et sünkroonida NTLM-ja Kerberose autentimise jaoks nõutavad parooli hashud.

Kui Azure AD Connect on konfigureeritud, siis sünkroonitakse ka kohapealne konto loomise või parooli muutmise sündmus ja seejärel sünkroonitakse pärand parooli hashes Azure AD. Lisateavet leiate [siit](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) ja juhised selle kohta, kuidas lubada AZURE AD DS Hybrid keskkonnas parooli sünkroonimine.