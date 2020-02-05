---
title: Viivitused SharePointi ja OneDrive ' i teatiste vastuvõtmisel
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771211"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="d8f77-102">Viivitused SharePointi ja OneDrive ' i teatiste vastuvõtmisel</span><span class="sxs-lookup"><span data-stu-id="d8f77-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="d8f77-103">Esmalt kontrollige oma e-posti kausta Rämpspost või rämpspost.</span><span class="sxs-lookup"><span data-stu-id="d8f77-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="d8f77-104">Kui **Kõik teatised mitmest failist või teekidest on hilinenud**, külastage [teenuse tervise armatuurlauda](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) , et kontrollida mis tahes teateid/intsidente, mis võivad esineda SharePointiga või Exchange ' iga.</span><span class="sxs-lookup"><span data-stu-id="d8f77-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="d8f77-105">See probleem võib olla koos SharePointi hoiatuse võimalusega või viivitused e-kirjade kaudu Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8f77-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="d8f77-106">Samuti Pange tähele, kas muud e-posti toimetatakse – kui mitte, probleem on tõenäoline, et Exchange viivitused.</span><span class="sxs-lookup"><span data-stu-id="d8f77-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="d8f77-107">Kui **konkreetse faili või teegi konkreetset teatist ei toimetata kohale**, proovige see kustutada ja uuesti luua.</span><span class="sxs-lookup"><span data-stu-id="d8f77-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="d8f77-108">Teatise uuestilaadamiseks vaadake teemat [SharePointi teatiste haldamine, vaatamine või kustutamine](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="d8f77-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="d8f77-109">Teatisi ei saa levirühmale saata.</span><span class="sxs-lookup"><span data-stu-id="d8f77-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="d8f77-110">Toetatakse ainult turbe-ja O365-rühmi.</span><span class="sxs-lookup"><span data-stu-id="d8f77-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="d8f77-111">Teatiste meilimalle ei saa kohandada.</span><span class="sxs-lookup"><span data-stu-id="d8f77-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="d8f77-112">Nende saavutamiseks peate kasutama Microsoft Flow või SharePoint Designeri töövoogu.</span><span class="sxs-lookup"><span data-stu-id="d8f77-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
