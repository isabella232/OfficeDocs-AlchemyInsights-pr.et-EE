---
title: Värskendage DNS-i kirjeid, et hoida oma veebisaiti praeguse majutusteenuse pakkuja juures
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827510"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="ffb80-102">Värskendage DNS-i kirjeid, et hoida oma veebisaiti praeguse majutusteenuse pakkuja juures</span><span class="sxs-lookup"><span data-stu-id="ffb80-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="ffb80-103">Avage Microsoft 365 halduskeskuses leht **Domeenide** häälestamine ja valige domeenide loendis domeen, mida  >  [](https://admin.microsoft.com/Adminportal#/Domains) oma veebisaidi jaoks kasutate.</span><span class="sxs-lookup"><span data-stu-id="ffb80-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="ffb80-104">Valige **+ Uus kohandatud kirje** ja sisestage järgmine teave.</span><span class="sxs-lookup"><span data-stu-id="ffb80-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ffb80-105">**DNS-i tüübi jaoks** **sisestage: A (Aadress)**</span><span class="sxs-lookup"><span data-stu-id="ffb80-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="ffb80-106">Tippige **väljale Hosti nimi või Pseudonüüm** järgmine tekst. **@**</span><span class="sxs-lookup"><span data-stu-id="ffb80-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="ffb80-107">**Tippige IP-aadressi** jaoks oma veebisaidi staatiline IP-aadress, kus seda praegu majutatakse (nt 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="ffb80-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="ffb80-108">See peab olema veebisaidi  *staatiline*  IP-aadress, mitte  *dünaamiline*  IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="ffb80-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="ffb80-109">Kontrollige veebisaiti, kus teie veebisaiti majutatakse, veendumaks, et saate oma avaliku veebisaidi jaoks staatilise IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="ffb80-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="ffb80-110">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="ffb80-110">Select **Save**.</span></span>

<span data-ttu-id="ffb80-111">Lisaks saate luua CNAME-kirje, et aidata klientidel teie veebisaiti leida.</span><span class="sxs-lookup"><span data-stu-id="ffb80-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="ffb80-112">Valige **+ Uus kohandatud kirje** ja sisestage järgmine teave.</span><span class="sxs-lookup"><span data-stu-id="ffb80-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="ffb80-113">**DNS-i tüübi jaoks** **sisestage: CNAME (Pseudonüüm)**</span><span class="sxs-lookup"><span data-stu-id="ffb80-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="ffb80-114">Hostinime **või pseudonüümi** korral tippige järgmine tekst: **www**</span><span class="sxs-lookup"><span data-stu-id="ffb80-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="ffb80-115">Tippige väljale Points to address (Points **to address)** oma veebisaidi täielik domeeninimi (FQDN) (nt contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ffb80-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="ffb80-116">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="ffb80-116">Select **Save**.</span></span>
