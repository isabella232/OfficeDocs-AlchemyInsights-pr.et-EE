---
title: Domeeni teenuse sünkroonimine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885152"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="75d3c-102">Domeeni teenuse sünkroonimine</span><span class="sxs-lookup"><span data-stu-id="75d3c-102">Domain service synchronization</span></span>

<span data-ttu-id="75d3c-103">Azure Active Directory Domain Services (Azure AD DS) hallatav domeeni objekte ja mandaate saab luua kohalikus domeenis või sünkroonitud Azure Active Directory (Azure AD) rentniku kaudu.</span><span class="sxs-lookup"><span data-stu-id="75d3c-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="75d3c-104">Kui te esimest korda juurutate Azure AD DS-i, konfigureeritakse ja käivitatakse automaatne kahesuunaline sünkroonimine Azure AD objektide jäljendamiseks.</span><span class="sxs-lookup"><span data-stu-id="75d3c-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="75d3c-105">See ühe suuna sünkroonimine jätkub taustal, et hoida Azure AD DS-i hallatavat domeeni ajakohane, mis tahes muudatuste Azure AD kaudu.</span><span class="sxs-lookup"><span data-stu-id="75d3c-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="75d3c-106">Azure AD DS-ist ei sünkroonita Azure AD.</span><span class="sxs-lookup"><span data-stu-id="75d3c-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="75d3c-107">Lisateavet Azure Active Directory domeeni teenuse sünkroonimise kohta leiate teemast [Domain Service sync](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="75d3c-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
