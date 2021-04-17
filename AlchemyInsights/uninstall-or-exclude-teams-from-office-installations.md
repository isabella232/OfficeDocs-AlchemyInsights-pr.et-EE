---
title: Teamsi desinstallimine või välistamine Office'i installidest
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827788"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="8cc1c-102">Teamsi desinstallimine või välistamine uutest või olemasolevatest Office'i installidest</span><span class="sxs-lookup"><span data-stu-id="8cc1c-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="8cc1c-103">Microsoft Teams on kaasatud microsoft 365 ettevõtterakenduste, Microsoft 365 ettevõtterakenduste ja Office for Maci rakenduste hulka.</span><span class="sxs-lookup"><span data-stu-id="8cc1c-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="8cc1c-104">Office'i [juurutustööriista abil](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) saate Teamsi Office'i uutest installidest välja jätta.</span><span class="sxs-lookup"><span data-stu-id="8cc1c-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="8cc1c-105">Teamsi *desinstallimiseks* Windowsiga seadmest lugege teemat [Microsoft Teamsi desinstallimine.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="8cc1c-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="8cc1c-106">Microsoft Teamsi puhastamiseks mitmest sihtarvutist või -kasutajast lugege [teemat Microsoft Teamsi juurutuse puhastamine.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="8cc1c-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="8cc1c-107">Suvandi [PreventTeamsInstall (PreventTeamsInstall)](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) abil saate takistada Microsoft Teamsi automaatset installimist Office'is.</span><span class="sxs-lookup"><span data-stu-id="8cc1c-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="8cc1c-108">Enne *Teamsi* installimist kasutage suvandit [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) et microsoft Teams ei käivituks pärast installimist automaatselt.</span><span class="sxs-lookup"><span data-stu-id="8cc1c-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="8cc1c-109">Kui kasutate Office for Maci, lugege teemat [Microsoft Teamsi installid Mac-arvutisse.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="8cc1c-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>