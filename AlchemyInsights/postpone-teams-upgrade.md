---
title: Teamsi ülemineku edasilükkamine
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741767"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="eb71e-102">Microsoft orienteeritud Teamsi versiooni edasi lükkamine</span><span class="sxs-lookup"><span data-stu-id="eb71e-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="eb71e-103">**Oluline**: selle probleemi lahendamiseks saate kasutada tugiteenuste diagnostikat, kuid tundub, et te ei kasuta uut administreerimiskeskuset.</span><span class="sxs-lookup"><span data-stu-id="eb71e-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="eb71e-104">Uue administreerimiskeskuse kasutamiseks libistage paremas ülanurgas olevale ülemisele paremale, mis ütleb, et **Uus halduskeskus** asub paremal.</span><span class="sxs-lookup"><span data-stu-id="eb71e-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="eb71e-105">Kui kasutate uut Administreerimiskeskuset, klõpsake nuppu **Vajad abi?** vidinat, tippige käsk "töörühma uuendamine edasi" ja seejärel järgige diagnostika käivitamiseks viipasid.</span><span class="sxs-lookup"><span data-stu-id="eb71e-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="eb71e-106">Kui saite teate Microsofti juhitud automatiseeritud ülemineku kohta Skype ' i ärirakendusest Microsoft Teamsi ja te soovite automaatse ülemineku hilisemale kuupäevale edasi lükata, saab üldadministraator sisse logida [teamsi administraatori portaali](https://admin.teams.microsoft.com/dashboard) ja pärast nupu **Värskenda olekut** klõpsamist jaotises Microsoft teamsi täiendus valida nupp **Lükka edasi** .</span><span class="sxs-lookup"><span data-stu-id="eb71e-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="eb71e-107">Kui soovite vaadata oma rentniku automaatse ülemineku uut kuupäeva Microsoft Teamsi, värskendage Teamsi administraatori portaali lehte.</span><span class="sxs-lookup"><span data-stu-id="eb71e-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="eb71e-108">**Märkus:** Nupp **Lükka edasi** on saadaval ainult juhul, kui olete saanud sõnumikeskuse teatise automatiseeritud versiooni kohta.</span><span class="sxs-lookup"><span data-stu-id="eb71e-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="eb71e-109">Globaalsed administraatorid saavad kasutada ka [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , et saada lisateavet nende praeguse täienduse oleku kohta.</span><span class="sxs-lookup"><span data-stu-id="eb71e-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
