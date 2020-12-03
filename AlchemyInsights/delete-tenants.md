---
title: Rentniku kustutamine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564485"
---
# <a name="delete-tenant"></a>Rentniku kustutamine

Azure ' i reklaami kustutamiseks veenduge järgmist.
- Olete kataloogis globaalse administraatorina.
- Te pole sisse logitud kontoga, mille vaikekaustana (nt contoso.onmicrosoft.com) on sisse logitud konto (nt admin@contoso.onmicrosoft.com).
- Eemaldage enne kustutamist kõik kataloogis olevad aktiivsed rakendused. Aktiivsete rakenduste eemaldamiseks liikuge rakenduse registreerimistele ja eemaldage olemasolevad rakendused.
- Ühtegi Microsoft Online ' i teenust (nt Microsoft Azure ' i, Office 365 või Azure AD Premiumi, mis on seotud kataloogiga) pole ühtegi aktiivset paketti. Edastage oma tellimused või kiirendage aktiivsete tellimuste tühistamist Azure ' i toe ja arvelduse kaudu. Lugege lisateavet Office ' i 365 ja Azure ' i tellimuste tühistamise kohta. Lisateavet rentniku jaoks olemasoleva tellimuse seostamise või lisamise kohta leiate teemast Azure ' i [reklaami rentniku jaoks Azure ' i tellimuse lisamine või lisamine](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Aktiivset litsentsi pole. Litsentside eemaldamise kohta leiate teavet teemast [tellimuse eemaldamine litsentsi eemaldamiseks](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Kui proovite Azure ' i reklaami kustutada, pole kataloogis ühtegi teist aktiivset kasutajat peale enda kui globaalse administraatorina. Eemaldada kõik muud aktiivsed kasutajad ja kõik rentniku kohandatud domeeninimega seotud sõltuvused tuleb eemaldada ka siis, kui admin@contoso.com on loodud kasutajad.

Üksikasjalikumad juhised selle kohta, kuidas:
- Kustutage "Azure Active Directory" või "tellimus", lugege teemat [Azure Active Directory kustutamine](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Rakenduste eemaldamine kataloogist leiate teavet teemast [Rakenduste eemaldamine](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
