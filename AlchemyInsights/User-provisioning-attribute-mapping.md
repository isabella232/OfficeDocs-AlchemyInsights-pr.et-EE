---
title: Kasutaja-ettevalmistamine atribuutide vastendamine
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
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949699"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="81f12-102">Kasutaja-ettevalmistamine atribuutide vastendamine</span><span class="sxs-lookup"><span data-stu-id="81f12-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="81f12-103">Atribuutide teadaolevate probleemide tõrkeotsingu kohta leiate teavet artiklist [atribuutide vastendamine](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="81f12-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="81f12-104">Microsoft Azure Active Directory (AD) pakub tuge kasutajate ettevalmistamisel kolmanda osapoole (nt Sales Force, G Suite jt) jaoks.</span><span class="sxs-lookup"><span data-stu-id="81f12-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="81f12-105">Kui lubate kasutaja ettevalmistamine kolmanda osapoole SaaS-rakenduse jaoks, kontrollib Azure ' i portaal selle atribuudi väärtusi atribuutide vastenduste kaudu.</span><span class="sxs-lookup"><span data-stu-id="81f12-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="81f12-106">Atribuutide vaike-vastenduste kohandamise kohta leiate teavet teemast [kasutajate ettevalmistamise atribuutide vastendamine rakenduses Azure Active Directory olevate Saas-vastenduste jaoks](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="81f12-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="81f12-107">Lisateavet SaaS app kasutaja ettevalmistamine kohta leiate teemast [mis on automatiseeritud Saas app kasutaja ettevalmistamine AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="81f12-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="81f12-108">Atribuudi-vastenduste kohandamisel kasutaja ettevalmistamiseks võite leida, et atribuuti, mida soovite vastendada, ei kuvata loendis Allikas atribuuti.</span><span class="sxs-lookup"><span data-stu-id="81f12-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="81f12-109">Teie kohapealses [Active Directorys oleva atribuudi sünkroonimine AZURE ad-sse rakenduse artikli ettevalmistamisel](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) näitab, kuidas lisada puuduvat atribuuti, kui sünkroonite selle oma KOHAPEALSEst ad-st Azure ' i ad-ga.</span><span class="sxs-lookup"><span data-stu-id="81f12-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
