---
title: Teamsi privaatse kanali kustutamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438989"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="51cfe-102">Teamsi privaatse kanali kustutamine</span><span class="sxs-lookup"><span data-stu-id="51cfe-102">Delete a Teams private channel</span></span>

<span data-ttu-id="51cfe-103">Microsoft on sellest probleemist teada saanud, kui teil on SharePointi säilituspoliitika aluseks oleva SharePointi saidi jaoks lubatud SharePointi säilituspoliitika.</span><span class="sxs-lookup"><span data-stu-id="51cfe-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="51cfe-104">Microsoft töötab lahendusega.</span><span class="sxs-lookup"><span data-stu-id="51cfe-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="51cfe-105">Vahepeal saate privaatse kanali kustutamiseks kasutada järgmisi lahendusi.</span><span class="sxs-lookup"><span data-stu-id="51cfe-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="51cfe-106">**Välistage meeskonna/saidikogumi SharePointi säilituspoliitika.**</span><span class="sxs-lookup"><span data-stu-id="51cfe-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="51cfe-107">Avage Office 365 administraatorite portaal ja valige Vasakpoolsel navigeerimispaanil **Kuva kõik** .</span><span class="sxs-lookup"><span data-stu-id="51cfe-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="51cfe-108">Valige jaotises **administraatori keskused**turbe- **& nõuetele vastavuse**  >  **vältimise**  >  **poliitika**.</span><span class="sxs-lookup"><span data-stu-id="51cfe-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="51cfe-109">Tuvastage mis tahes poliitika, mis rakendub SharePointi saitidele, ja muutke poliitikat, nii et privaatset kanalit sisaldava meeskonna SharePointi saiti ei kaasata säilituspoliitika alla.</span><span class="sxs-lookup"><span data-stu-id="51cfe-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="51cfe-110">Salvesta poliitika.</span><span class="sxs-lookup"><span data-stu-id="51cfe-110">Save the policy.</span></span>
    <span data-ttu-id="51cfe-111">Poliitika sätete jõustumiseks võib kuluda kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="51cfe-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="51cfe-112">Kui sait on välja jäetud, saate privaatse kanali kustutada.</span><span class="sxs-lookup"><span data-stu-id="51cfe-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="51cfe-113">Võimalik ***, et saate privaatse*** kanali kustutada, kasutades Microsoft teamsi oma Androidi seadmes.</span><span class="sxs-lookup"><span data-stu-id="51cfe-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="51cfe-114">Seostuva SharePointi teabe leiate teemast [SharePoint Online ' is või OneDrive for Businessis ei saa üksusi kustutada](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="51cfe-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>