---
title: Tellimuse juurdepääs
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807293"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Azure ' i probleemide tõttu ei saa Azure ' i sisse logida (brauser hangub, keerutab, ei laadi jne).

Võib juhtuda, et seisak mõjutab katkestust. Palun kontrolli, kas käimas on katkestus: [Azure ' i tervislik seisund](https://status.azure.com/status/history/).

Logige kõik aktiivsed Azure ' i seansid välja. Alustage oma veebibrauseri privaatset või inkognito režiimi.

Samuti võite proovida värskendada brauserit, kasutada mõnda muud brauserit, kustutada vahemälu küpsised, kui need ei tööta.

Lisateave: [Sisselogimistega seotud probleemide tõrkeotsing](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Tellimusele ei pääse juurde**

Veenduge, et [Azure ' i portaalis](https://portal.azure.com/)oleks valitud õige Azure ' i kataloog paremas ülanurgas olevast kontost.

Veenduge, et [Azure ' i konto keskuses](https://account.windowsazure.com/Subscriptions)oleks konto administraator.

Lisateave: [leitud tellimuste tõrkeotsing](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Arvelduste ajaloole ei saa juurde pääseda**

Konto administraator peab veenduma, et arvelduse teabe kasutajaks olev kasutaja on lisatud Azure Active Directorysse külalisena kasutajana: [uue kasutaja lisamine või kustutamine](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Seejärel peab kasutajale andma üldise administraatori rolli: [määrata kasutajatele rolli](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Postitage see, kasutaja saab anda arvelduse juurdepääsu RBAC poliitika kaudu: [anda juurdepääsu Arveldusele](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Soovitatavad dokumendid**

-   [Ma ei saa oma Azure ' i tellimuse haldamiseks sisse logida](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)