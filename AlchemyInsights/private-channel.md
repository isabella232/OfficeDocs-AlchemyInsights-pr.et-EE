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
# <a name="private-channels-in-microsoft-teams"></a>Privaatkanalid Microsoft Teamsi

Privaatkanalid on Microsoft Teamsi uus funktsioon. Pange tähele, et privaatseid kanaleid ei saa teisendada standardkanalites ega vastupidi.

Privaatkanalite (nt teave [privaatkanalite loomise ja liikmesuse](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) ning [privaatkanali SharePointi saitide](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)kohta) üksikasjade kohta vaadake [Microsoft teamsi privaatseid kanaleid](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Märkus:** Kuna privaatkanali sõnumite säilitamise konfiguratsioon ei ole veel toetatud, rentnike Säilituspoliitikad lubatud ei ole privaatne kanalid vaikimisi lubatud. Privaatseid kanaleid saab lubada meeskondade halduskeskuses. Samuti pidage meeles, et kuigi privaatkanalite sõnumite säilitamist ei toetata, toetatakse privaatkanalite ühiskasutusse antud failide säilitamist.

**Vajad uut meeskonna omanikku?**

Kui teie privaatkanali omanik lahkub, saate lisada uue meeskonna omaniku meeskondade PowerShelli kaudu.


- [siia](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , et installida meeskonnad PowerShelli.

Siin on cmdlet teil on vaja:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Lisateavet meeskondade PowerShelli kohta leiate jaotisest [Teamsi PowerShelli ülevaade](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
