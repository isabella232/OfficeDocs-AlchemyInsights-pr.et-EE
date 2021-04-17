---
title: AllowSelfServicePurchase'i poliitikat ei saa seada ega vaadata
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826087"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="0aa73-102">AllowSelfServicePurchase'i poliitikat ei saa seada ega vaadata</span><span class="sxs-lookup"><span data-stu-id="0aa73-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="0aa73-103">Kui proovite seada või vaadata AllowSelfServicePurchase'i poliitikat, kuvatakse järgmine tõrketeade:</span><span class="sxs-lookup"><span data-stu-id="0aa73-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="0aa73-104">*HandleError : Tootepoliitika toomine poliitikaga "AllowSelfServicePurchase", ErrorMessage nurjus – aluseks olev ühendus suleti: saatmisel ilmnes ootamatu tõrge.*</span><span class="sxs-lookup"><span data-stu-id="0aa73-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="0aa73-105">Põhjuseks võib olla transpordikihi turbe (TLS) vanem versioon.</span><span class="sxs-lookup"><span data-stu-id="0aa73-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="0aa73-106">MSCommerce'i teenuse ühendamiseks peate kasutama TLS 1.2 või suuremat versiooni.</span><span class="sxs-lookup"><span data-stu-id="0aa73-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="0aa73-107">TLS-protokolli lubamiseks/1.2 lubamiseks,kinnitamiseks ja uuesti proovimiseks proovige järgmisi juhiseid.</span><span class="sxs-lookup"><span data-stu-id="0aa73-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="0aa73-108">Sisestage PowerShelli käsuviibale (PS C) järgmine käsk, et \) määrata TLS-protokolliks versioon 1.2.</span><span class="sxs-lookup"><span data-stu-id="0aa73-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="0aa73-109">Kontrollige, kas TLS-protokoll(id) on kasutusel, järgmise käsuga:</span><span class="sxs-lookup"><span data-stu-id="0aa73-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="0aa73-110">Vajaduse korral saate uuesti käivitada käsud Too või Värskenda.</span><span class="sxs-lookup"><span data-stu-id="0aa73-110">Retry the Get or Update commands as needed.</span></span>

