---
title: Yammeri administraatorid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 03/22/2021
ms.locfileid: "51035731"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="e5024-102">Yammeri administraatorid</span><span class="sxs-lookup"><span data-stu-id="e5024-102">About Yammer admins</span></span>

<span data-ttu-id="e5024-103">**Võrgu administraatorid**</span><span class="sxs-lookup"><span data-stu-id="e5024-103">**Network admins**</span></span>

<span data-ttu-id="e5024-104">Globaalsed administraatorid edutatakse automaatselt Yammeri võrgus kinnitatud administraatori rolliks.</span><span class="sxs-lookup"><span data-stu-id="e5024-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="e5024-105">Järgmistel juhtudel ei pruugi see edutamine õigesti juhtuda.</span><span class="sxs-lookup"><span data-stu-id="e5024-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="e5024-106">On olemas mitu Yammeri võrku ja administraator on sisse logitud valesse.</span><span class="sxs-lookup"><span data-stu-id="e5024-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="e5024-107">[Võrgu konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) on vajalik ühe Yammeri võrgu juurde pääsemiseks.</span><span class="sxs-lookup"><span data-stu-id="e5024-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="e5024-108">Kasutatakse Azure PIM-i.</span><span class="sxs-lookup"><span data-stu-id="e5024-108">Azure PIM is being used.</span></span> <span data-ttu-id="e5024-109">Kasutaja ei pruugi olla edutatud üldisele administraatorile piisavalt kaua, et edutamine toimuks.</span><span class="sxs-lookup"><span data-stu-id="e5024-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="e5024-110">Yammeri tulevane värskendus võib selle probleemi lahendada, kuid see on kõige parem, kui soovite kasutajad globaalsele administraatorile käsitsi lisada.</span><span class="sxs-lookup"><span data-stu-id="e5024-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="e5024-111">Yammeri võrguga on sünkroonimise probleem olemas.</span><span class="sxs-lookup"><span data-stu-id="e5024-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="e5024-112">Sellisel juhul on täiendavaks uurimiseks vaja tugiteenuste taotlust.</span><span class="sxs-lookup"><span data-stu-id="e5024-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="e5024-113">Yammeri administraatori rollide kohta leiate lisateavet teemast [Yammeri administraatorite haldamine](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span><span class="sxs-lookup"><span data-stu-id="e5024-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="e5024-114">**Rühma administraatorid**</span><span class="sxs-lookup"><span data-stu-id="e5024-114">**Group admins**</span></span>

<span data-ttu-id="e5024-115">Rühma administraatorid Microsoft 365 ühendatud rühmadega sünkroonitakse Azure AD rühma liikmestaatusega.</span><span class="sxs-lookup"><span data-stu-id="e5024-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="e5024-116">Suurte rühmade korral võib sünkroonimine võtta pikema aja.</span><span class="sxs-lookup"><span data-stu-id="e5024-116">For large groups, this sync can take an extended period.</span></span>
