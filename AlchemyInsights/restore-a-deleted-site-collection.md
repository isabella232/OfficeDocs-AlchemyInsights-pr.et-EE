---
title: Kustutatud saidi taastamine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692039"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="6e6db-102">Kustutatud saidi taastamine</span><span class="sxs-lookup"><span data-stu-id="6e6db-102">Restore a deleted site</span></span>

<span data-ttu-id="6e6db-103">Kui administraator kustutab SharePointi saidi, paigutatakse see saidikogumi prügikasti, kus seda säilitatakse 93 päeva jooksul, enne kui see jäädavalt kustutatakse.</span><span class="sxs-lookup"><span data-stu-id="6e6db-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="6e6db-104">Saidi taastamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="6e6db-104">To restore the site:</span></span>
  
1. <span data-ttu-id="6e6db-105">Klõpsake uues SharePointi administreerimiskeskuses lindil nuppu **Prügikast** .</span><span class="sxs-lookup"><span data-stu-id="6e6db-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="6e6db-106">Märkige selle saidikogumi kõrval olev ruut, mille soovite taastada.</span><span class="sxs-lookup"><span data-stu-id="6e6db-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="6e6db-107">Klõpsake nuppu **Taasta kustutatud üksused**.</span><span class="sxs-lookup"><span data-stu-id="6e6db-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="6e6db-108">Kustutatud suhtluse saidi taastamiseks saate kasutada uut SharePointi halduskeskus.</span><span class="sxs-lookup"><span data-stu-id="6e6db-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="6e6db-109">Vastasel juhul peate kasutama Microsoft PowerShelli.</span><span class="sxs-lookup"><span data-stu-id="6e6db-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="6e6db-110">Microsoft 365 rühma kuuluva saidi taastamiseks peate Exchange ' i administreerimiskeskuses rühma taastama.</span><span class="sxs-lookup"><span data-stu-id="6e6db-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="6e6db-111">Rühmi saab taastada 30 päeva jooksul pärast kustutamist.</span><span class="sxs-lookup"><span data-stu-id="6e6db-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

