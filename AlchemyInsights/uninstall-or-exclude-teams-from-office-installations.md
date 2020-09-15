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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Uutest või olemasolevatest Office ' i installist meeskondade desinstallimine või välistamine

Microsoft Teams on kaasatud Microsoft 365 rakendustesse Enterprise, Microsoft 365 Apps for Office ja Office for Mac.

- Office ' i [juurutamise tööriista](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) abil saate meeskonnad uutest Office ' i installist eemaldada.
- Töörühmade *desinstallimiseks* seadmes, kus töötab Windows, lugege teemat [Microsoft teamsi desinstallimine](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Microsoft Teamsi puhastamiseks mitmest targetist või kasutajast leiate teavet teemast [Microsoft teamsi juurutuse puhastamine](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Kasutage funktsiooni [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , et takistada Microsoft teamsi automaatset installimist Office ' iga.
- Kasutage funktsiooni [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *enne kui meeskonnad on installitud*, et takistada Microsoft teamsi automaatset käivitumist pärast installimist.

Kui kasutate teenusekomplekti Office for Mac, lugege teemat [Microsoft teamsi installid Mac-arvutis](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).