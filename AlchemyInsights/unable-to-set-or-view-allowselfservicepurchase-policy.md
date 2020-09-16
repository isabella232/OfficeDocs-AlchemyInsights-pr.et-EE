---
title: AllowSelfServicePurchase poliitikat ei saa seada ega vaadata
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735195"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="0a7ce-102">AllowSelfServicePurchase poliitikat ei saa seada ega vaadata</span><span class="sxs-lookup"><span data-stu-id="0a7ce-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="0a7ce-103">Kui proovite määrata või vaadata AllowSelfServicePurchase poliitikat, kuvatakse järgmine tõrketeade:</span><span class="sxs-lookup"><span data-stu-id="0a7ce-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="0a7ce-104">*HandleError: PolicyId ' AllowSelfServicePurchase ', sündmustelogist-ga tootepoliitika toomine nurjus: saatmisel ilmnes ootamatu tõrge.*</span><span class="sxs-lookup"><span data-stu-id="0a7ce-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="0a7ce-105">See võib olla tingitud transpordikihi turbe (TLS) varasemast versioonist.</span><span class="sxs-lookup"><span data-stu-id="0a7ce-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="0a7ce-106">MSCommerce teenusega ühenduse loomiseks peate kasutama TLS 1,2 või uuemat versiooni.</span><span class="sxs-lookup"><span data-stu-id="0a7ce-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="0a7ce-107">Toimige järgmiselt, et lubada/seadistada TLS-protokoll 1,2, kinnitada ja uuesti proovida.</span><span class="sxs-lookup"><span data-stu-id="0a7ce-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="0a7ce-108">PowerShelli käsureal (PS C: \) Sisestage järgmine KÄSK TLS-protokolli versioonile 1,2 määramiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="0a7ce-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="0a7ce-109">Kontrollige, kas TLS-protokoll (ID) on kasutusel, ja kasutage järgmist käsku.</span><span class="sxs-lookup"><span data-stu-id="0a7ce-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="0a7ce-110">Proovige käske Too või Värskenda uuesti vastavalt vajadusele.</span><span class="sxs-lookup"><span data-stu-id="0a7ce-110">Retry the Get or Update commands as needed.</span></span>

