---
title: Värskendage DNS-kirjete hoida oma kodulehel praeguse hosting pakkuja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665756"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="9a094-102">Värskendage DNS-kirjete hoida oma kodulehel praeguse hosting pakkuja</span><span class="sxs-lookup"><span data-stu-id="9a094-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="9a094-103">Microsoft 365 halduskeskus, lehele **setup**  >  [Domeenid](https://portal.office.com/adminportal/home#/Domains) ja domeenide loendis Valige domeen, mida kasutate oma veebilehel.</span><span class="sxs-lookup"><span data-stu-id="9a094-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="9a094-104">Valige **+ Uus kohandatud kirje** ja sisestage järgmine:</span><span class="sxs-lookup"><span data-stu-id="9a094-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9a094-105">Sisestage **DNS-i tüüp** : **a (aadress)**</span><span class="sxs-lookup"><span data-stu-id="9a094-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="9a094-106">**Hosti nime või pseudonüümi**, tippige järgmine:**@**</span><span class="sxs-lookup"><span data-stu-id="9a094-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="9a094-107">**IP-aadressi**puhul tippige oma veebisaidi staatiline IP-aadress, kus see praegu majutatud (nt 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="9a094-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="9a094-108">See peab olema *staatiline* IP-aadress veebilehel, mitte *dünaamiline* IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="9a094-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="9a094-109">Kontrollige saiti, kus teie veebisait on majutatud veendumaks, et saate oma avaliku veebisaidi jaoks staatilise IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="9a094-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="9a094-110">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="9a094-110">Select **Save**.</span></span>

<span data-ttu-id="9a094-111">Lisaks saate luua CNAME-kirje, et aidata klientidel teie veebisaiti leida.</span><span class="sxs-lookup"><span data-stu-id="9a094-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="9a094-112">Valige **+ Uus kohandatud kirje** ja sisestage järgmine:</span><span class="sxs-lookup"><span data-stu-id="9a094-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9a094-113">Sisestage **DNS-i tüüp** : **CNAME (alias)**</span><span class="sxs-lookup"><span data-stu-id="9a094-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="9a094-114">**Hosti nime või pseudonüümi**, tippige järgmine: **www**</span><span class="sxs-lookup"><span data-stu-id="9a094-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="9a094-115">**Aadressi punktide käsitlemiseks**tippige oma veebisaidile täielik DOMEENINIMI (FQDN) (nt contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9a094-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="9a094-116">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="9a094-116">Select **Save**.</span></span>
