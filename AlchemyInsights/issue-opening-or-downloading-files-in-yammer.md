---
title: Probleem failide avamisel või allalaadimisel Yammeris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148248"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Probleem failide avamisel või allalaadimisel Yammeris

Klassikaline Yammer toetab sõnumitesse ja rühmadesse failide üleslaadimise mitut suvandit. Sõltuvalt võrgu konfiguratsioonist on failide vaikemälu SharePointis.

Uue Yammeri failivalija ei toeta veel kõiki klassikalises Yammeris saadaolevaid suvandeid. Tulevane värskendus lisab täiendavaid funktsioone. Lisateavet leiate teemast [Faili või pildi manustamine Yammeri vestluse postitusse](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Faili ei saa avada ega alla laadida**  

Fail võib yammerisse üles laadida, kuid linkida ka SharePoint Online'i failiga. Tõrkeotsingu sooritamiseks peate esmalt määrama faili asukoha. Kui fail on Yammerisse üles laaditud, on sellel URL *.yammer.com. Veenduge, et nõutavad URL-id ja IP-aadressid on blokeeritud. Lisateavet leiate ajaveebipostitusest [Yammeri püsiprogrammeeritud IP-aadresside kasutamine pole soovitatav.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Kontrollige, kas faili saab alla laadida ka üldadministraator. Kui fail on privaatne, peate võib-olla kasutama privaatse sisu režiimi. Lisateavet leiate teemast [Yammeri privaatse sisu jälgimine](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammeri võrgutasandi külalised ja failid SharePoint Online'is**  

[Yammeri võrgutasandi külalised](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ei kasuta Azure AD B2B ja on Yammeri teenuse sisemine, et nad ei pääse Yammeri failidele, mis on talletatud SharePointis. Looge väline AAD B2B kasutaja, kellel on juurdepääs dokumenditeekidele SharePoint Online'is, kasutades seda identiteeti. Lisateavet Yammeri tulevase Azure AD B2B külalistoe kohta leiate teemast [Ettevõttest ettevõtteni (B2B) külaline yammeri eelvaates – klienditingimused ja KKK](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).