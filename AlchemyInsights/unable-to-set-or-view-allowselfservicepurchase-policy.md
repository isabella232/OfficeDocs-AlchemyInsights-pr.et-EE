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
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158557"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="6d245-102">Ei saa seada või vaadata AllowSelfServicePurchase poliitika</span><span class="sxs-lookup"><span data-stu-id="6d245-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="6d245-103">Kui proovite seada või vaadata AllowSelfServicePurchase poliitika, kuvatakse järgmine tõrketeade:</span><span class="sxs-lookup"><span data-stu-id="6d245-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="6d245-104">*HandleError: tootepoliitika hankimine poliitika ID ' AllowSelfServicePurchase ', ErrorMessage-aluseks olev ühendus suleti: saatmisel ilmnes ootamatu tõrge.*</span><span class="sxs-lookup"><span data-stu-id="6d245-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="6d245-105">See võib olla tingitud vanem versioon transpordikihi turbe (TLS).</span><span class="sxs-lookup"><span data-stu-id="6d245-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="6d245-106">MSCommerce teenuse ühendamiseks peate kasutama TLS 1,2 või uuem.</span><span class="sxs-lookup"><span data-stu-id="6d245-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="6d245-107">Proovige/seadke TLS-i protokoll 1,2, kontrollige ja proovige järgmisi samme.</span><span class="sxs-lookup"><span data-stu-id="6d245-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="6d245-108">PowerShelli Käsuviip (PS C:\) sisestage järgmine käsk, et määrata TLS-i protokolli versioon 1,2:</span><span class="sxs-lookup"><span data-stu-id="6d245-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="6d245-109">Veenduge, et TLS-protokoll (ID) kasutusel, järgmine käsk:</span><span class="sxs-lookup"><span data-stu-id="6d245-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="6d245-110">Proovige vajadusel käsku Võta või uuenda.</span><span class="sxs-lookup"><span data-stu-id="6d245-110">Retry the Get or Update commands as needed.</span></span>

