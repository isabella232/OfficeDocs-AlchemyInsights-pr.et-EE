---
title: Värskendage DNS-i kirjeid, et hoida oma veebisait praeguse majutusteenuse pakkujaga.
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815781"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="2ce44-102">Värskendage DNS-i kirjeid, et hoida oma veebisait praeguse majutusteenuse pakkujaga.</span><span class="sxs-lookup"><span data-stu-id="2ce44-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="2ce44-103">Avage Microsoft 365 halduskeskus leht **Häälesta**  >  [Domeenid](https://admin.microsoft.com/Adminportal#/Domains) ja valige domeenide loendist domeen, mida kasutate oma veebisaidi jaoks.</span><span class="sxs-lookup"><span data-stu-id="2ce44-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="2ce44-104">Valige **+ Uus kohandatud kirje** ja sisestage järgmine tekst.</span><span class="sxs-lookup"><span data-stu-id="2ce44-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="2ce44-105">**DNS-i tüübi** sisestamiseks sisestage: **a (aadress)**</span><span class="sxs-lookup"><span data-stu-id="2ce44-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="2ce44-106">Tippige väljale **hosti nimi või pseudonüüm**järgmine tekst. **@**</span><span class="sxs-lookup"><span data-stu-id="2ce44-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="2ce44-107">**IP-aadressi**korral tippige veebisaidi staatiline IP-aadress, kus see on praegu majutatud (nt 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="2ce44-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="2ce44-108">See peab olema veebisaidi  *staatiline*  IP-aadress, mitte  *dünaamiline*  IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="2ce44-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="2ce44-109">Kontrolli saidil, kus teie veebisait on majutatud, et saaksite oma avaliku veebisaidi jaoks staatilise IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="2ce44-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="2ce44-110">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="2ce44-110">Select **Save**.</span></span>

<span data-ttu-id="2ce44-111">Lisaks saate luua CNAME-kirje, mis aitab klientidel teie veebisaiti leida.</span><span class="sxs-lookup"><span data-stu-id="2ce44-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="2ce44-112">Valige **+ Uus kohandatud kirje** ja sisestage järgmine tekst.</span><span class="sxs-lookup"><span data-stu-id="2ce44-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="2ce44-113">**DNS-i tüübi** sisestamiseks sisestage: **CNAME (pseudonüüm)**</span><span class="sxs-lookup"><span data-stu-id="2ce44-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="2ce44-114">Tippige väljale **hosti nimi või pseudonüüm**järgmine tekst: **www**</span><span class="sxs-lookup"><span data-stu-id="2ce44-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="2ce44-115">**Punktide**saamiseks tippige oma veebisaidi täielik DOMEENINIMI (FQDN) (nt contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2ce44-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="2ce44-116">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="2ce44-116">Select **Save**.</span></span>
