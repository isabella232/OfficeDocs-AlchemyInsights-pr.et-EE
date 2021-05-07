---
title: Lisandmoodulite juurutamine Microsoft 365 rakendused
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233518"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="0f677-102">Lisandmoodulite juurutamine Microsoft 365 rakendused</span><span class="sxs-lookup"><span data-stu-id="0f677-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="0f677-103">Tsentraliseeritud juurutamine on soovitatav viis Office juurutada oma asutuse kasutajatele ja rühmadele lisandmooduleid.</span><span class="sxs-lookup"><span data-stu-id="0f677-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="0f677-104">Lisandmoodulite juurutamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="0f677-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="0f677-105">**Märkus.** Lisandmoodulite installimiseks üksikkasutajana Office lugege teemat Lisandmoodulite vaatamiseks, haldamiseks ja [installimiseks Office programmides.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="0f677-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="0f677-106">Samuti veenduge, et Office store'i lisandmoodulite individuaalne hankimine oleks lubatud.</span><span class="sxs-lookup"><span data-stu-id="0f677-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="0f677-107">Lisateavet leiate teemast Lisandmoodulite allalaadimise keelamine, kui lülitate Office poe välja [(v.a Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="0f677-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="0f677-108">Veenduge, et teie keskkond vastaks tsentraliseeritud juurutuse abil lisandmoodulite juurutamise nõuetele.</span><span class="sxs-lookup"><span data-stu-id="0f677-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="0f677-109">Lisateavet leiate teemast [Nõuded](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="0f677-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="0f677-110">Lisandmoodulite **Sätted**  >  **avage**  >   Microsoft 365 rakenduste toomine.</span><span class="sxs-lookup"><span data-stu-id="0f677-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="0f677-111">Märkmed:</span><span class="sxs-lookup"><span data-stu-id="0f677-111">Notes:</span></span> 

- <span data-ttu-id="0f677-112">Integreeritud rakenduste kasutamiseks peab administraatoril olema üldadministraatori või Exchange administraatoriõigused.</span><span class="sxs-lookup"><span data-stu-id="0f677-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="0f677-113">Kui juurutate lisandmooduleid mitmele kasutajale, soovitame teha ülesandeid üksikute kasutajate asemel rühmade abil.</span><span class="sxs-lookup"><span data-stu-id="0f677-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="0f677-114">Lisateavet leiate teemast Lisandmooduli määramise kaalutlused [kasutajatele ja rühmadele.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="0f677-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="0f677-115">Tsentraliseeritud juurutus ei toeta pesastatud rühmade või emarühmadega rühmade kasutajaid.</span><span class="sxs-lookup"><span data-stu-id="0f677-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="0f677-116">Lisateavet leiate teemast [Kasutaja ja rühma ülesanded.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="0f677-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="0f677-117">Veenduge, et Microsoft 365-rakendusehaldusteenus (GUID: "0517ffae-825d-4aff-999e-3f2336b8a20a") oleks sisse logimiseks lubatud.</span><span class="sxs-lookup"><span data-stu-id="0f677-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="0f677-118">Lisateavet leiate teemast [Rakenduse atribuutide konfigureerimine.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="0f677-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="0f677-119">Kui teil on probleeme lisandmoodulite juurutamisel integreeritud rakenduste abil, proovige juurutada [lisandmoodulite abil.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="0f677-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="0f677-120">Lisateavet leiate järgmistest teemadest.</span><span class="sxs-lookup"><span data-stu-id="0f677-120">For more information, see:</span></span>

<span data-ttu-id="0f677-121">[Lisandmoodulite juurutamine halduskeskuses](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Lisandmoodulite haldamine halduskeskuses](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Lisandmoodulite haldamine tsentraliseeritud juurutuse PowerShelli cmdlet-käskude abil](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Avaldage Office lisandmoodulid tsentraliseeritud juurutuse abil Microsoft 365 halduskeskuse kaudu](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Tõrkeotsing. Kasutaja ei näe lisandmooduleid](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Kasutajate tõrgete tõrkeotsing Office lisandmoodulitega](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="0f677-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>