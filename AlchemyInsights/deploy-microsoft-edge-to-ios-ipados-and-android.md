---
title: Microsoft Edge ' i juurutamine iOS-i, iPadOS ja Androidi jaoks
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194481"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="f959c-102">Microsoft Edge ' i juurutamine iOS-i, iPadOS ja Androidi jaoks</span><span class="sxs-lookup"><span data-stu-id="f959c-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="f959c-103">Alltoodud juhendav stsenaarium aitab teil iOS-i, iPadOS ja Androidi seadmete kasutajatele määrata Microsoft Edge ' i.</span><span class="sxs-lookup"><span data-stu-id="f959c-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="f959c-104">Kui blokeerite kasutajatele mobiilsideseadmete registreerimise, siis see juhendav stsenaarium ei tööta ja kasutajad peavad Microsoft Edge ' i ise installima.</span><span class="sxs-lookup"><span data-stu-id="f959c-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="f959c-105">Juhendav stsenaarium koosneb järgmistest etappidest.</span><span class="sxs-lookup"><span data-stu-id="f959c-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="f959c-106">Eeltingimused</span><span class="sxs-lookup"><span data-stu-id="f959c-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="f959c-107">Tutvustus</span><span class="sxs-lookup"><span data-stu-id="f959c-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="f959c-108">Põhitõed</span><span class="sxs-lookup"><span data-stu-id="f959c-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="f959c-109">Konfiguratsiooni</span><span class="sxs-lookup"><span data-stu-id="f959c-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="f959c-110">Ülesanded</span><span class="sxs-lookup"><span data-stu-id="f959c-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="f959c-111">Läbivaatus ja loomine</span><span class="sxs-lookup"><span data-stu-id="f959c-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="f959c-112">Kui olete juhendava stsenaariumi juhiseid täitnud, siis Microsoft Intune ' i poliitikad võimaldavad Microsoft Edge ' i ärirakenduse järgmisi funktsioone.</span><span class="sxs-lookup"><span data-stu-id="f959c-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="f959c-113">Kahekordne identiteet</span><span class="sxs-lookup"><span data-stu-id="f959c-113">Dual identity</span></span>
- <span data-ttu-id="f959c-114">Integreeritus Microsoft Intune ' i rakenduse kaitsmise poliitikaga</span><span class="sxs-lookup"><span data-stu-id="f959c-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="f959c-115">Integreerimine Azure Active Directory rakenduse puhverserveriga</span><span class="sxs-lookup"><span data-stu-id="f959c-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="f959c-116">Hallatavate lemmikute ja avalehe kiirklahvid</span><span class="sxs-lookup"><span data-stu-id="f959c-116">Managed favorites and home page shortcuts</span></span>
