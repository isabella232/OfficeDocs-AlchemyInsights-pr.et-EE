---
title: Orvuks kasutaja kustutamine asutusesisesest serverist
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197940"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Orvuks kasutaja kustutamine asutusesisesest serverist

Orvuks kasutaja eemaldamiseks toimige järgmiselt.

1. Sundida kataloogi sünkroonimine, järgides juhiseid [Mis on hübriid identiteedi Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Kataloogi sünkroonimise kontrollimiseks vaadake teemat [Mis on hübriididentiteet Azure Active Directoryga?](https://technet.microsoft.com/library/jj151797.aspx)

3. Kui sünkroonimine toimib õigesti, kuid Active Directory objekti kustutamine ei levi Azure AD, käsitsi eemaldada orvuks objekti, kasutades ühte järgmistest Azure Active Directory moodul Windows PowerShelli cmdlet-käsud:

    Eemalda MsolContact  
    Eemalda MsolGroup  
    Eemalda MsolUser

    Näiteks orvuks kasutaja ID john.smith@contoso.com eemaldamiseks, mis loodi algselt kataloogi sünkroonimise abil, käivitage cmdlet-käsk:

    Eemalda MsolUser –UserPrincipalName John.Smith@Contoso.com