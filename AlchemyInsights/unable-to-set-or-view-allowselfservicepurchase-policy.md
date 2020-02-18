---
title: Ei saa seada või vaadata AllowSelfServicePurchase poliitika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091690"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="ed135-102">Ei saa seada või vaadata AllowSelfServicePurchase poliitika</span><span class="sxs-lookup"><span data-stu-id="ed135-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="ed135-103">Kui proovite seada või vaadata AllowSelfServicePurchase poliitika, kuvatakse järgmine tõrketeade:</span><span class="sxs-lookup"><span data-stu-id="ed135-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="ed135-104">*HandleError: tootepoliitika hankimine poliitika ID ' AllowSelfServicePurchase ', ErrorMessage-aluseks olev ühendus suleti: saatmisel ilmnes ootamatu tõrge.*</span><span class="sxs-lookup"><span data-stu-id="ed135-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="ed135-105">See võib olla tingitud vanem versioon transpordikihi turbe (TLS).</span><span class="sxs-lookup"><span data-stu-id="ed135-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="ed135-106">MSCommerce teenuse ühendamiseks peate kasutama TLS 1,2 või uuem.</span><span class="sxs-lookup"><span data-stu-id="ed135-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="ed135-107">Proovige/seadke TLS-i protokoll 1,2, kontrollige ja proovige järgmisi samme.</span><span class="sxs-lookup"><span data-stu-id="ed135-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="ed135-108">PowerShelli Käsuviip (PS C:\) sisestage järgmine käsk, et määrata TLS-i protokolli versioon 1,2:</span><span class="sxs-lookup"><span data-stu-id="ed135-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="ed135-109">\[Net. ServicePointManager]:: SecurityProtocol = \[net. SecurityProtocolType]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="ed135-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="ed135-110">Veenduge, et TLS-protokoll (ID) kasutusel, järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="ed135-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="ed135-111">\[Net. ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="ed135-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="ed135-112">Proovige vajadusel käsku Võta või uuenda.</span><span class="sxs-lookup"><span data-stu-id="ed135-112">Retry the Get or Update commands as needed.</span></span>

