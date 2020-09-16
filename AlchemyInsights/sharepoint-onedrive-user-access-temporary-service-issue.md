---
title: Jõudluse probleemid – SharePoint või OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771240"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="b2695-102">SharePointi või OneDrive ' i aeglased, kättesaamatud või kättesaamatud mitme kasutaja jaoks</span><span class="sxs-lookup"><span data-stu-id="b2695-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="b2695-103">Kui OneDrive ' i või SharePointi sait pole saadaval mitmele kasutajale, kellel oli varem juurdepääs, võib olla ajutine teenuse probleem.</span><span class="sxs-lookup"><span data-stu-id="b2695-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="b2695-104">[Kontrollige teenuse tervise armatuurlauda](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b2695-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="b2695-105">**Kasutaja lisamine ja litsentsimine**</span><span class="sxs-lookup"><span data-stu-id="b2695-105">**Add and license the user**</span></span>

<span data-ttu-id="b2695-106">Veenduge, et [määrate kasutajatele Microsoft 365 ettevõtetele litsentsid](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="b2695-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="b2695-107">**Õiguse määramine**</span><span class="sxs-lookup"><span data-stu-id="b2695-107">**Assign Permissions**</span></span>

<span data-ttu-id="b2695-108">Kui kasutajale on määratud SharePointi litsents ja ta saab endiselt juurdepääsu keelava sõnumi, siis veenduge, et neil on määratud [õigusetasemed](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="b2695-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="b2695-109">**Accessi taotluse funktsiooni kasutamine**</span><span class="sxs-lookup"><span data-stu-id="b2695-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="b2695-110">[Accessi taotluse funktsioon](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) võimaldab inimestel taotleda juurdepääsu sisule, mida neil praegu ei ole.</span><span class="sxs-lookup"><span data-stu-id="b2695-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="b2695-111">**Kohandatud skripti lubamine võib põhjustada juurdepääsu keelatud probleemidele**</span><span class="sxs-lookup"><span data-stu-id="b2695-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="b2695-112">On teatud stsenaariumid, mille korral saab *kohandatud skripti funktsiooni lubada* , kui juurdepääs on keelatud.</span><span class="sxs-lookup"><span data-stu-id="b2695-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="b2695-113">Mõjutatud funktsioonide loendi, turvalisuse kaalutlused ja funktsiooni keelamise võimalus.</span><span class="sxs-lookup"><span data-stu-id="b2695-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="b2695-114">Vaadake teemat [kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b2695-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

