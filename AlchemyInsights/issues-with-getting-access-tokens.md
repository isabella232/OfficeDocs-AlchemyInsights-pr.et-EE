---
title: Juurdepääsu märkide hankimisega seotud probleemid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7776"
- "9004351"
ms.openlocfilehash: e2d15603835d3fb43df1b6b5dadec64af00290ff
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916835"
---
# <a name="issues-with-getting-access-tokens"></a><span data-ttu-id="d9ef9-102">Juurdepääsu märkide hankimisega seotud probleemid</span><span class="sxs-lookup"><span data-stu-id="d9ef9-102">Issues with getting access tokens</span></span>

<span data-ttu-id="d9ef9-103">Selles teemas käsitletakse tõrkeid, mille abil saate ressursile juurde pääseda Accessi märkide hankimiseks.</span><span class="sxs-lookup"><span data-stu-id="d9ef9-103">This topic deals with failures to acquire access tokens to access a resource.</span></span>

<span data-ttu-id="d9ef9-104">**Mul on probleeme töötamise alustamisega**</span><span class="sxs-lookup"><span data-stu-id="d9ef9-104">**I'm having trouble getting started**</span></span>

<span data-ttu-id="d9ef9-105">Probleemide lahendamiseks, mis ilmnevad siis, kui proovite alustada, lugege järgmisi artikleid.</span><span class="sxs-lookup"><span data-stu-id="d9ef9-105">To troubleshoot issues you encounter when trying to get started, see the following articles:</span></span>

- [<span data-ttu-id="d9ef9-106">Ma ei leia alustamiseks koodi näidist</span><span class="sxs-lookup"><span data-stu-id="d9ef9-106">I can't find a code sample to get started</span></span>](https://docs.microsoft.com/azure/active-directory/develop/sample-v2-code) 
- [<span data-ttu-id="d9ef9-107">Vajan abi .NET-i loa saamiseks</span><span class="sxs-lookup"><span data-stu-id="d9ef9-107">I need help getting a token in .NET</span></span>](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)

<span data-ttu-id="d9ef9-108">**Ma ei tea, kuidas taotleda ja kasutada märke**</span><span class="sxs-lookup"><span data-stu-id="d9ef9-108">**I don't know how to request and use tokens**</span></span>

<span data-ttu-id="d9ef9-109">Juhiseid märkide taotlemise ja kasutamise kohta leiate järgmistest artiklitest.</span><span class="sxs-lookup"><span data-stu-id="d9ef9-109">For guidance on how to request and use tokens, see the following articles:</span></span>

- [<span data-ttu-id="d9ef9-110">Ma ei tea, kuidas taotleda loa koodi</span><span class="sxs-lookup"><span data-stu-id="d9ef9-110">I don’t know how to request an authorization code</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code) 
- [<span data-ttu-id="d9ef9-111">Ma ei tea, kuidas taotleda juurdepääsuluba</span><span class="sxs-lookup"><span data-stu-id="d9ef9-111">I don’t know how to request an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-authorization-code-to-request-an-access-token) 
- [<span data-ttu-id="d9ef9-112">Ma ei tea, kuidas kasutada ressursile juurdepääsemiseks juurdepääsuluba</span><span class="sxs-lookup"><span data-stu-id="d9ef9-112">I don’t know how to use an access token to access a resource</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token-to-access-the-resource) 
- [<span data-ttu-id="d9ef9-113">Ma ei tea, kuidas juurdepääsuluba värskendada</span><span class="sxs-lookup"><span data-stu-id="d9ef9-113">I don’t know how to refresh an access token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refreshing-the-access-tokens)

<span data-ttu-id="d9ef9-114">**Mul on tõendi taotlemisel viga**</span><span class="sxs-lookup"><span data-stu-id="d9ef9-114">**I got an error while requesting a token**</span></span>

<span data-ttu-id="d9ef9-115">Loa taotlemisel ilmnenud tõrgete tõrkeotsing leiate järgmistest artiklitest.</span><span class="sxs-lookup"><span data-stu-id="d9ef9-115">To troubleshoot errors you have encountered while requesting for a token, see the following articles:</span></span>

- [<span data-ttu-id="d9ef9-116">Sain loa taotlemisel tõrketeate</span><span class="sxs-lookup"><span data-stu-id="d9ef9-116">I received a service error when requesting a token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- [<span data-ttu-id="d9ef9-117">Ma saan uue tõrketeate varem töötava rakenduse jaoks</span><span class="sxs-lookup"><span data-stu-id="d9ef9-117">I'm getting a new error to a previously working app</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-breaking-changes)

<span data-ttu-id="d9ef9-118">**Lisateavet AADSTS kohta leiate teemast tõrkekoodidest.**</span><span class="sxs-lookup"><span data-stu-id="d9ef9-118">**How do I get more information about AADSTS error codes?**</span></span>

<span data-ttu-id="d9ef9-119">Lisateavet leiate teemast [autentimine ja autoriseerimise tõrkekoodid](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).</span><span class="sxs-lookup"><span data-stu-id="d9ef9-119">For more information, see [Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).</span></span>





