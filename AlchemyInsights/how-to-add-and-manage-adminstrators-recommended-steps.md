---
title: Administraatorite lisamine ja haldamine – soovitatavad juhised
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339028"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Administraatorite lisamine ja haldamine – soovitatavad juhised

Teie probleemi kirjelduse põhjal oleme teie jaoks lahenduse leidnud. Enamik kliente suutis pärast meie dokumentatsiooni järgimist oma probleemi ise lahendada.

**Tellimuse administraatori või kaasadministraatori redigeerimine**

- Kontoadministraator saab mõlemat rolli redigeerida, kuid tellimuse administraator saab muuta ainult Azure'i portaali [kaasadministraatoreid.](https://ms.portal.azure.com/#home)
- [Azure'i tellimuse administraatorite lisamine või muutmine](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Tellimuse administraatori või Co-Administrator (AIRS) tellimuste värskendamine**

Teenuseadministraator või kaasadministraator saab seda toimingut ise teha, järgides järgmisi juhiseid.

1. Logige sisse [Azure'i portaali ja](https://ms.portal.azure.com/#home) klõpsake vasakus **noas nuppu Kuluhaldus +** Arveldamine.
2. Klõpsake tellimusega reaüksust. See avab tellimuse ülevaate.
3. Klõpsake **laba Tellimus** nuppu **Atribuudid.** 
4. Klõpsake nuppu **Teenuseadministraator.**
5. Sisestage selle kasutaja meiliaadress, kelle soovite määrata teenuseadministraatoriks, ja klõpsake nuppu **OK**.

**Kaasadministraatori lisamine/ muutmine/eemaldamine**

1. Logige Azure'i [portaali sisse](https://ms.portal.azure.com/#home) teenuseadministraatorina.
2. Avage [tellimused](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ja valige tellimus. (Kaasadministraatoreid saab määrata ainult tellimuse ulatuses.)
3. Liikuge **Accessi juhtelemendi (IAM)** klassikaliste administraatorite juurde Lisa kaasadministraator, et avada paan Lisa kaasadministraator (kui suvand Lisa kaasadministraator on keelatud, tähistab see, et teil  >    >    >   pole õigusi). 
4. Valige kasutaja, kelle soovite lisada, ja klõpsake **nuppu Lisa.**

**Lisateave:**
- [Kaasadministraatori lisamine](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Kaasadministraatori eemaldamine](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Teenuseadministraatori muutmine](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Kontoadministraatori vaade](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Juurdepääsu haldamine RBAC-i ja Azure'i portaali abil](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Kasutajate lisamine ja kustutamine Azure Active Directory (AD) abil**

Saate lisada uusi kasutajaid või kustutada olemasolevaid kasutajaid oma Azure Active Directory (Azure AD) organisatsioonist.

1. Uue kasutaja lisamiseks logige azure'i portaali sisse ettevõtte kasutajaadministraatorina. [](https://ms.portal.azure.com/#home)
2. Valige **Azure Active Directory**, valige **Kasutajad ja** seejärel klõpsake nuppu Uus **kasutaja**.
3. Sisestage **lehel** Kasutaja nõutav teave. Klõpsake **nuppu Loo**. Kasutaja luuakse ja lisatakse teie Azure AD rentnikule.

**Lisateave:**

- [Uue kasutaja lisamine](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Kasutaja kustutamine](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Kasutaja profiiliteabe lisamine või värskendamine Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Soovitatud dokumendid**

- [Mis on rollipõhine juurdepääsukontroll (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Azure'i erinevate rollide mõistmine](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Administraatori rolliõigused Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Õppetükk: RBAC-i ja Azure'i portaali abil kasutajale juurdepääsu andmine](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Azure'i RBAC-i tõrkeotsing](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Ressursside rühmi saab korraldada Azure'i haldusrühmade abil.](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Azure'i arve koopia taotlemine meili teel](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Krediit- või deebetkaardi lisamine, värskendamine või eemaldamine Azure'ist](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Tellimuse haldamine (uuesti aktiveerimine/tühistamine/vahetamine)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



