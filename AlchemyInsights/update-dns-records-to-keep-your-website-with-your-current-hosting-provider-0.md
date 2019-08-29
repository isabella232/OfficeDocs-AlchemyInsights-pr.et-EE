---
title: Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665756"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="86f15-102">Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust</span><span class="sxs-lookup"><span data-stu-id="86f15-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="86f15-103">Minge Microsoft 365 administreerimiskeskuses **Seadistus** > [domeenide](https://portal.office.com/adminportal/home#/Domains) lehekülg ja domeenide loendis valige domeeni kasutamisel oma veebilehel.</span><span class="sxs-lookup"><span data-stu-id="86f15-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="86f15-104">Valige **+ uue kohandatud kirje** ja tippige järgmine:</span><span class="sxs-lookup"><span data-stu-id="86f15-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="86f15-105">Sisestage **DNS-i tüüp** : **(aadress)**</span><span class="sxs-lookup"><span data-stu-id="86f15-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="86f15-106">**Hosti nimi või pseudonüüm**, tippige järgmine:**@**</span><span class="sxs-lookup"><span data-stu-id="86f15-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="86f15-107">**IP-aadress**tippige veebisaidi, kus on praegu majutatud (näiteks 172.16.140.1) staatiline IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="86f15-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="86f15-108">See peab olema koduleht, mitte *dünaamilise* IP-aadressi *staatilise* IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="86f15-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="86f15-109">Kohas, kus teie koduleheküljel on hostitud veendumaks, et avaliku veebisaidi staatilisi IP-aadressi saamiseks pöörduge.</span><span class="sxs-lookup"><span data-stu-id="86f15-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="86f15-110">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="86f15-110">Select **Save**.</span></span>

<span data-ttu-id="86f15-111">Lisaks saate luua CNAME-kirje aitab kasutajatel leida oma veebilehel.</span><span class="sxs-lookup"><span data-stu-id="86f15-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="86f15-112">Valige **+ uue kohandatud kirje** ja tippige järgmine:</span><span class="sxs-lookup"><span data-stu-id="86f15-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="86f15-113">Sisestage **DNS-i tüüp** : **CNAME (pseudonüüm)**</span><span class="sxs-lookup"><span data-stu-id="86f15-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="86f15-114">**Hosti nimi või pseudonüüm**, tippige järgmine: **www**</span><span class="sxs-lookup"><span data-stu-id="86f15-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="86f15-115">**Punktid aadressile**, tippige domeeni nimi (FQDN) oma veebilehel (nt contoso.com).</span><span class="sxs-lookup"><span data-stu-id="86f15-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="86f15-116">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="86f15-116">Select **Save**.</span></span>
