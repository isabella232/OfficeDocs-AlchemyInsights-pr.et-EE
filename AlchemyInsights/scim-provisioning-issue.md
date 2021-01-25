---
title: SCIM ettevalmistamise probleem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949714"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="1acb4-102">SCIM ettevalmistamise probleem</span><span class="sxs-lookup"><span data-stu-id="1acb4-102">SCIM provisioning issue</span></span>

<span data-ttu-id="1acb4-103">Automaatne ettevalmistamine viitab kasutajate identiteedi ja rollide loomisele pilveteenuse rakendustes, millele kasutajad vajavad juurdepääsu.</span><span class="sxs-lookup"><span data-stu-id="1acb4-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="1acb4-104">Lisaks kasutaja identiteedi loomisele sisaldab automaatne ettevalmistamine kasutajate identiteedi hooldust ja eemaldamist oleku või rollide muutmisena.</span><span class="sxs-lookup"><span data-stu-id="1acb4-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="1acb4-105">Enne juurutuse alustamist saate vaadata, [Kuidas ettevalmistamine töötab](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) , et saada teada, kuidas Azure Active DIRECTORY (ad) säte töötab, ja hankida konfiguratsiooni soovitusi.</span><span class="sxs-lookup"><span data-stu-id="1acb4-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="1acb4-106">Rakenduse arendajana saate kasutada süsteemi domeeni identiteedi halduseks (SCIM), et lubada kasutajate ja rühmade automaatset ettevalmistamist rakenduse ja Azure AD vahel.</span><span class="sxs-lookup"><span data-stu-id="1acb4-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="1acb4-107">[SCIM lõpp-punkti koostamine ja kasutaja ettevalmistamine AZURE ad](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) artiklis kirjeldab, kuidas luua SCIM lõpp ja integreerida see Azure AD ettevalmistamise teenusega.</span><span class="sxs-lookup"><span data-stu-id="1acb4-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



