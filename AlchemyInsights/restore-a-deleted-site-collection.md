---
title: Kustutatud saidi taastamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582231"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="a8a25-102">Kustutatud saidi taastamine</span><span class="sxs-lookup"><span data-stu-id="a8a25-102">Restore a deleted site</span></span>

<span data-ttu-id="a8a25-103">Kui administraator kustutab SharePointi saidi, paigutatakse see saidikogumi prügikasti, kus seda säilitatakse 93 päeva enne jäädavalt kustutamist.</span><span class="sxs-lookup"><span data-stu-id="a8a25-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="a8a25-104">Saidi taastamiseks toimige järgmiselt.</span><span class="sxs-lookup"><span data-stu-id="a8a25-104">To restore the site:</span></span>
  
1. <span data-ttu-id="a8a25-105">Klõpsake uue SharePointi administreerimiskeskus lindi **prügikasti** .</span><span class="sxs-lookup"><span data-stu-id="a8a25-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="a8a25-106">Märkige selle saidikogumi kõrval olev ruut, mida soovite taastada.</span><span class="sxs-lookup"><span data-stu-id="a8a25-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="a8a25-107">Klõpsake käsul **Taasta kustutatud üksused**.</span><span class="sxs-lookup"><span data-stu-id="a8a25-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="a8a25-108">Kustutatud suhtlussaidi taastamiseks võite kasutada uut SharePointi administreerimiskeskust.</span><span class="sxs-lookup"><span data-stu-id="a8a25-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="a8a25-109">Vastasel juhul peate kasutama Microsoft PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="a8a25-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="a8a25-110">Saidi, mis kuulub Microsoft 365 rühma taastamiseks peate taastama rühma Exchange ' i halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="a8a25-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="a8a25-111">Rühmi saab taastada 30 päeva pärast nende kustutamist.</span><span class="sxs-lookup"><span data-stu-id="a8a25-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

