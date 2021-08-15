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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993889"
---
# <a name="delete-tenant"></a>Rentniku kustutamine

Azure AD kustutamiseks veenduge, et:
- Olete kataloogi üldadministraator.
- Te pole sisse logitud kontoga, kus on vaikekataloog (nt contoso.onmicrosoft.com on sisse logitud kontol (nt admin@contoso.onmicrosoft.com).
- Eemaldage enne kustutamist kataloogist kõik aktiivsed rakendused. Aktiivsete rakenduste eemaldamiseks liikuge jaotisse Rakenduse registreerimised ja eemaldage olemasolevad rakendused.
- Kataloogiga seotud Microsoft Online'i teenuste (nt Microsoft Azure, Office 365 Või Azure AD Premium jaoks pole aktiivseid tellimusi. Azure'i toe ja arveldamise kaudu saate oma tellimused üle kanda või aktiivsete tellimuste tühistamise kiirendada. Lugege lisateavet selle kohta, kuidas Office 365 Azure'i tellimused tühistada. Juhised rentnikuga olemasoleva tellimuse seostamise või lisamise kohta leiate teemast [Azure AD rentnikuga Azure'i](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)tellimuse seostamine või lisamine.
- Aktiivset litsentsi pole. Litsentside eemaldamise kohta leiate teavet [teemast Litsentsi eemaldamise tellimuse eemaldamine.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Azure AD kustutamise katsel pole kataloogis muid aktiivseid kasutajaid peale teie kui üldadministraatori. Eemaldage kõik muud aktiivsed kasutajad ja kõik rentniku kohandatud domeeninime sõltuvused tuleb eemaldada (nt kasutajaid, kes on loodud admin@contoso.com).

Üksikasjalikumad juhised selle kohta, kuidas teha järgmist.
- Kustutage "Azure Active Directory" või "tellimus", lugege [teemat Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Rakenduste eemaldamine kataloogist leiate teemast [Rakenduste eemaldamine.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
