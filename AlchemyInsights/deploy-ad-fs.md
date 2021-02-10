---
title: AD FS-i juurutamine
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177442"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="f3b50-102">AD FS-i juurutamine</span><span class="sxs-lookup"><span data-stu-id="f3b50-102">Deploy AD FS</span></span>

<span data-ttu-id="f3b50-103">Active Directory Federation Services (AD FS) juurutamine kasutab teie kohapealset infrastruktuuri kasutajate autentimiseks Office 365 teenuste jaoks.</span><span class="sxs-lookup"><span data-stu-id="f3b50-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="f3b50-104">Välise sisselogimise korral saate lubada kasutajatel logida Office 365 teenustesse ja tarkvarasse sisse Azure Active Directoryga (Azure AD) integreeritud rakendustena.</span><span class="sxs-lookup"><span data-stu-id="f3b50-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f3b50-105">Väline sisselogimine kinnitab kasutajad teie kohapealse Active Directory kaudu AD FS-i kaudu.</span><span class="sxs-lookup"><span data-stu-id="f3b50-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="f3b50-106">Ka ettevõtte võrgus ei nõuta kasutajatelt paroolide uuesti sisestamist.</span><span class="sxs-lookup"><span data-stu-id="f3b50-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="f3b50-107">[AD FS-i juurutuse nõunik](https://go.microsoft.com/fwlink/?linkid=2071178) pakub üksikasjalikke juhiseid kohapealse AD FS-i infrastruktuuri juurutamiseks, mis autentib Microsoft 365 ja Office 365 teenuste kasutajaid.</span><span class="sxs-lookup"><span data-stu-id="f3b50-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="f3b50-108">Selle juhendi abil saab teie ettevõte üle vaadata AD FS-i komponente ja nõudeid, hankida ja installida SSL-sertifikaate, mis on juurutamiseks vajalikud, ning installida vajalik veebirakenduse puhverserver.</span><span class="sxs-lookup"><span data-stu-id="f3b50-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
