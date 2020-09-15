---
title: Teamsi Office ' i installide desinstallimine või välistamine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658217"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="c7a43-102">Uutest või olemasolevatest Office ' i installist meeskondade desinstallimine või välistamine</span><span class="sxs-lookup"><span data-stu-id="c7a43-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="c7a43-103">Microsoft Teams on kaasatud Microsoft 365 rakendustesse Enterprise, Microsoft 365 Apps for Office ja Office for Mac.</span><span class="sxs-lookup"><span data-stu-id="c7a43-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="c7a43-104">Office ' i [juurutamise tööriista](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) abil saate meeskonnad uutest Office ' i installist eemaldada.</span><span class="sxs-lookup"><span data-stu-id="c7a43-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="c7a43-105">Töörühmade *desinstallimiseks* seadmes, kus töötab Windows, lugege teemat [Microsoft teamsi desinstallimine](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="c7a43-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="c7a43-106">Microsoft Teamsi puhastamiseks mitmest targetist või kasutajast leiate teavet teemast [Microsoft teamsi juurutuse puhastamine](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="c7a43-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="c7a43-107">Kasutage funktsiooni [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , et takistada Microsoft teamsi automaatset installimist Office ' iga.</span><span class="sxs-lookup"><span data-stu-id="c7a43-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="c7a43-108">Kasutage funktsiooni [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *enne kui meeskonnad on installitud*, et takistada Microsoft teamsi automaatset käivitumist pärast installimist.</span><span class="sxs-lookup"><span data-stu-id="c7a43-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="c7a43-109">Kui kasutate teenusekomplekti Office for Mac, lugege teemat [Microsoft teamsi installid Mac-arvutis](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="c7a43-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>