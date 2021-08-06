---
title: Juurdepääs tellimusele
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999236"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Brauseriprobleemide tõttu ei saa Azure'i sisse logida (brauser hangub, jätkab pöörlemist, ei laadi jne)

Teid võib mõjutada katkestus. Kontrollige, kas on käimas katkestus: [Azure'i seisund.](https://status.azure.com/status/history/)

Logige välja kõik aktiivsed Azure'i seansid. Käivitage veebibrauseri era- või inkognitorežiim.

Samuti võite proovida brauserit värskendada, kasutada mõnda muud brauserit, kustutada vahemäluküpsised, kui ülalpool ei tööta.

Lisateave: [Sisselogimisprobleemide tõrkeotsing](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Tellimustele ei pääse juurde**

Veenduge, [et Azure'i](https://portal.azure.com/)portaalis on paremal ülaservas kontolt valitud õige Azure'i kaust.

Veenduge [Azure'i](https://account.windowsazure.com/Subscriptions)kontokeskuses, kas kasutatud konto on konto administraator.

Lisateave: [Tellimusteta tõrkeotsing](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Arveldusajaloole ei pääse juurde**

Konto administraator peab veenduma, et kasutaja, kes kasutab arveldusteavet, lisatakse Azure Active'i kataloogi külaliskasutajana: [uue kasutaja lisamine või kustutamine.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Seejärel peab kasutajale olema antud üldadministraatori roll: [kasutajatele rolli määramine.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Postitage see, kasutajale saab arvelduse juurdepääsuks kasutada RBAC-poliitikaid: [juurdepääsu võimaldamine arveldusele.](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)

**Soovitatud dokumendid**

-   [Ma ei saa Azure'i tellimuse haldamiseks sisse logida](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)