---
title: Yammeri vaikedomeeni muutmine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817952"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="a6cea-102">Yammeri vaikimi/peamise domeeni muutmine</span><span class="sxs-lookup"><span data-stu-id="a6cea-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="a6cea-103">Yammeri URL sisaldab teie Yammeri võrgu praegust peamist domeeninime.</span><span class="sxs-lookup"><span data-stu-id="a6cea-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="a6cea-104">See domeeninimi ei tohi ühtida Office 365-s või Azure AD-s määratud peamise domeeninimega.</span><span class="sxs-lookup"><span data-stu-id="a6cea-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="a6cea-105">Rentnikule lisatud kohandatud domeenide arvu põhjal esineb käitumises erinevusi ja selle põhjal, kas Yammer on toetatud konfiguratsioonis (1 rentnik: 1 võrk või 1:1).</span><span class="sxs-lookup"><span data-stu-id="a6cea-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="a6cea-106">Saadaval on [Yammeri domeenide ja Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) dokumentatsioon.</span><span class="sxs-lookup"><span data-stu-id="a6cea-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="a6cea-107">Vale domeeni kuvamise kõige levinum põhjus on see, et olemas on mitu Yammeri võrku ja need tuleb konsolideerida.</span><span class="sxs-lookup"><span data-stu-id="a6cea-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="a6cea-108">[Üheks võrguks konsolideerimine](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) võrgu migreerimise tööriista kasutades on oluline esimene samm.</span><span class="sxs-lookup"><span data-stu-id="a6cea-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="a6cea-109">Tehke seda enne esmase domeeni määramise proovimist.</span><span class="sxs-lookup"><span data-stu-id="a6cea-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="a6cea-110">**Kohandatud domeenid puuduvad**</span><span class="sxs-lookup"><span data-stu-id="a6cea-110">**No custom domains**</span></span>

<span data-ttu-id="a6cea-111">Uute rentnike jaoks kasutatakse Yammeri jaoks rentniku vaikedomeeni (nt fabrikam.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="a6cea-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="a6cea-112">Peamiseks domeeniks on määratud yammer.com/fabrikam.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="a6cea-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="a6cea-113">**Üks kohandatud domeen**</span><span class="sxs-lookup"><span data-stu-id="a6cea-113">**Single custom domain**</span></span>

<span data-ttu-id="a6cea-114">Yammer valib automaatselt Yammeri peamiseks domeeniks rentniku kohandatud domeeni (nt fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="a6cea-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="a6cea-115">Selleks määratakse yammer.com/fabrikam.com.</span><span class="sxs-lookup"><span data-stu-id="a6cea-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="a6cea-116">Selle muudatuse teeb domeeni sünkroonimisteenus ja selleks jõustumiseks võib kuluda kuni 24 tundi.</span><span class="sxs-lookup"><span data-stu-id="a6cea-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="a6cea-117">**Mitu kohandatud domeeni**</span><span class="sxs-lookup"><span data-stu-id="a6cea-117">**Multiple custom domains**</span></span>

<span data-ttu-id="a6cea-118">Yammeril saab olla peamine domeen, mis erineb rentniku vaikedomeenist.</span><span class="sxs-lookup"><span data-stu-id="a6cea-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="a6cea-119">Kuna kohandatud domeene on mitu, ei proovi Yammer arvata, milline saadaolevatest on õige domeen.</span><span class="sxs-lookup"><span data-stu-id="a6cea-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="a6cea-120">Peate avama tugiteenuse juhtumi, et taotleda, et peamine domeeninimi muudetaks teie valitud peamiseks domeeniks.</span><span class="sxs-lookup"><span data-stu-id="a6cea-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="a6cea-121">**Täiendav tõrkeotsingu teave**</span><span class="sxs-lookup"><span data-stu-id="a6cea-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="a6cea-122">Mõnel juhul võivad domeenid olla rentnike vahel liikunud ja domeeni sünkroonimisteenus ei saanud korralikult töötada.</span><span class="sxs-lookup"><span data-stu-id="a6cea-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="a6cea-123">Lisaks valele peamisele domeenile võivad teil tekkida sisselogimise ja muud probleemid.</span><span class="sxs-lookup"><span data-stu-id="a6cea-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="a6cea-124">Selle probleemi lahendamiseks võib olla vajalik Microsofti tugiteenuste abiga domeenide liigutamine õigesse võrgustikku.</span><span class="sxs-lookup"><span data-stu-id="a6cea-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="a6cea-125">See olukord vajab otsest abistamist ja selle lahendamiseks võib kuluda veidi aega, eriti kui domeeninimede loend on väga pikk.</span><span class="sxs-lookup"><span data-stu-id="a6cea-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="a6cea-126">Avage seda tüüpi probleemide lahendamisl abi saamiseks tugiteenuse juhtum.</span><span class="sxs-lookup"><span data-stu-id="a6cea-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="a6cea-127">Tugiagendiga töötades nad kontrollivad, kas teie kontrolli all oleva rentniku domeenid on kinnitatud.</span><span class="sxs-lookup"><span data-stu-id="a6cea-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="a6cea-128">Nad võivad küsida täiendavaid kontrollküsimusi teie domeenide kohta, kui need on teie rentnikule lisatud, kuid pole DNS-i poolt kinnitatud.</span><span class="sxs-lookup"><span data-stu-id="a6cea-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="a6cea-129">Veenduge, et domeenid oleksid DNS-i poolt kinnitatud, et kiirendada protsessi.</span><span class="sxs-lookup"><span data-stu-id="a6cea-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
