---
title: Kustutatud Microsoft 365 rühma taastamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505682"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="4dc5a-102">Kustutatud Microsoft 365 rühma taastamine</span><span class="sxs-lookup"><span data-stu-id="4dc5a-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="4dc5a-103">Kustutatud Microsoft 365 rühma või Microsoft Teamsi saate taastada 30 päeva jooksul pärast kustutamist.</span><span class="sxs-lookup"><span data-stu-id="4dc5a-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="4dc5a-104">Microsoft 365 halduskeskusesse sisselogimiseks ning kustutatud rühmade ja töörühmade loendi vaatamiseks avage [Microsoft 365 halduskeskus.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="4dc5a-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="4dc5a-105">**Märkus.** Logige sisse rentnikuadministraatori või rühmaadministraatori rollile määratud kontoga.</span><span class="sxs-lookup"><span data-stu-id="4dc5a-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="4dc5a-106">Valige taastamiseks kustutatud Microsoft 365 rühm/Teams ja klõpsake nuppu **Taasta rühm**.</span><span class="sxs-lookup"><span data-stu-id="4dc5a-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="4dc5a-107">Kui rühma ei saa vastuoluliste SMTP-aadresside tõttu taastada, kasutage konflikti põhjustava objekti leidmiseks ja SMTP-aadressi eemaldamiseks järgmist käsku.</span><span class="sxs-lookup"><span data-stu-id="4dc5a-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="4dc5a-108">**Märkus.** Mõnel juhul võib rühma ja kõigi selle andmete taastamine võtta kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="4dc5a-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="4dc5a-109">Lisateavet powerShelli abil rühmade taastamise kohta leiate teemast Kustutatud [Microsoft 365 rühma taastamine.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="4dc5a-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>