---
title: Azure Active Directory läbimise autentimise konfigureerimine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035539"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="0ecbb-102">Azure Active Directory läbimise autentimise konfigureerimine</span><span class="sxs-lookup"><span data-stu-id="0ecbb-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="0ecbb-103">Siin on mõned juhised, mis aitavad teil konfigureerida läbima autentimise.</span><span class="sxs-lookup"><span data-stu-id="0ecbb-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="0ecbb-104">**Azure Active Directory ühenduse häälestamiseks** tehke järgmist. [kasutajate sünkroonimine kataloogiteenuse](https://admin.microsoft.com/AdminPortal/Home) abil aitab teil konfigureerida parooli Hash sünkroonimise või läbitud autentimise.</span><span class="sxs-lookup"><span data-stu-id="0ecbb-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="0ecbb-105">See konfiguratsioon võimaldab kasutajatel logida sisse oma e-posti ja asutusesisese Active Directory (domeenikontroller) sama parooliga.</span><span class="sxs-lookup"><span data-stu-id="0ecbb-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="0ecbb-106">[Teie kataloogiteenuse kasutajate sünkroonimisel](https://admin.microsoft.com/AdminPortal/Home) kehtib ka Federation sign-in for Active Directory Federation Services (AD FS).</span><span class="sxs-lookup"><span data-stu-id="0ecbb-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="0ecbb-107">**Azure ' i funktsioonide häälestamiseks tehke** järgmist. Azure ' i [ad setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) ' i abil saate häälestada Azure Active Directory põhifunktsioonid (nt rühma-põhise Accessi haldus, iseteeninduskeskuse parooli lähtestamine pilveteenuse rakenduste jaoks ja Azure Active Directory rakenduse puhverserveri asutusesisese veebirakenduse avaldamiseks).</span><span class="sxs-lookup"><span data-stu-id="0ecbb-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


