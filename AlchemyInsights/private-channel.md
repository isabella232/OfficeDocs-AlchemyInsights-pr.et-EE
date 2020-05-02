---
title: Privaatne kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005434"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="cfbe8-102">Privaatkanalid Microsoft Teamsi</span><span class="sxs-lookup"><span data-stu-id="cfbe8-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="cfbe8-103">Privaatkanalid on Microsoft Teamsi uus funktsioon.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="cfbe8-104">Pange tähele, et privaatseid kanaleid ei saa teisendada standardkanalites ega vastupidi.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="cfbe8-105">Privaatkanalite (nt teave [privaatkanalite loomise ja liikmesuse](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) ning [privaatkanali SharePointi saitide](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)kohta) üksikasjade kohta vaadake [Microsoft teamsi privaatseid kanaleid](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="cfbe8-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="cfbe8-106">**Märkus:** Kuna privaatkanali sõnumite säilitamise konfiguratsioon ei ole veel toetatud, rentnike Säilituspoliitikad lubatud ei ole privaatne kanalid vaikimisi lubatud.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="cfbe8-107">Privaatseid kanaleid saab lubada meeskondade halduskeskuses.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="cfbe8-108">Samuti pidage meeles, et kuigi privaatkanalite sõnumite säilitamist ei toetata, toetatakse privaatkanalite ühiskasutusse antud failide säilitamist.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="cfbe8-109">**Vajad uut meeskonna omanikku?**</span><span class="sxs-lookup"><span data-stu-id="cfbe8-109">**Need a new team owner?**</span></span>

<span data-ttu-id="cfbe8-110">Kui teie privaatkanali omanik lahkub, saate lisada uue meeskonna omaniku meeskondade PowerShelli kaudu.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="cfbe8-111">[siia](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , et installida meeskonnad PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="cfbe8-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="cfbe8-112">Siin on cmdlet teil on vaja:</span><span class="sxs-lookup"><span data-stu-id="cfbe8-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="cfbe8-113">Lisateavet meeskondade PowerShelli kohta leiate jaotisest [Teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="cfbe8-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
