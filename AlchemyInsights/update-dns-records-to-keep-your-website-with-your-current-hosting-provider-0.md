---
title: Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506403"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="5ca65-102">Värskendada DNS-kirjete hoida oma veebilehel koos oma praeguse hosting teenust</span><span class="sxs-lookup"><span data-stu-id="5ca65-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="5ca65-103">Valige leheküljel [Domeenid](https://portal.office.com/adminportal/home#/Domains) domeenide nimekirja domeeni kasutamisel oma veebilehel.</span><span class="sxs-lookup"><span data-stu-id="5ca65-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="5ca65-104">Valige **+ uue kohandatud kirje** ja tippige järgmine:</span><span class="sxs-lookup"><span data-stu-id="5ca65-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="5ca65-105">Sisestage **DNS-i tüüp** : **(aadress)**</span><span class="sxs-lookup"><span data-stu-id="5ca65-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="5ca65-106">**Hosti nimi või pseudonüüm**, tippige järgmine:**@**</span><span class="sxs-lookup"><span data-stu-id="5ca65-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="5ca65-107">**IP-aadress**tippige veebisaidi, kus on praegu majutatud (näiteks 172.16.140.1) staatiline IP-aadress.</span><span class="sxs-lookup"><span data-stu-id="5ca65-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="5ca65-108">See peab olema koduleht, mitte *dünaamilise* IP-aadressi *staatilise* IP-aadressi.</span><span class="sxs-lookup"><span data-stu-id="5ca65-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="5ca65-109">Kohas, kus teie koduleheküljel on hostitud veendumaks, et avaliku veebisaidi staatilisi IP-aadressi saamiseks pöörduge.</span><span class="sxs-lookup"><span data-stu-id="5ca65-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="5ca65-110">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="5ca65-110">Select **Save**.</span></span>

<span data-ttu-id="5ca65-111">Lisaks saate luua CNAME-kirje aitab kasutajatel leida oma veebilehel.</span><span class="sxs-lookup"><span data-stu-id="5ca65-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="5ca65-112">Valige **+ uue kohandatud kirje** ja tippige järgmine:</span><span class="sxs-lookup"><span data-stu-id="5ca65-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="5ca65-113">Sisestage **DNS-i tüüp** : **CNAME (pseudonüüm)**</span><span class="sxs-lookup"><span data-stu-id="5ca65-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="5ca65-114">**Hosti nimi või pseudonüüm**, tippige järgmine: **www**</span><span class="sxs-lookup"><span data-stu-id="5ca65-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="5ca65-115">**Punktid aadressile**, tippige domeeni nimi (FQDN) oma veebilehel (nt contoso.com).</span><span class="sxs-lookup"><span data-stu-id="5ca65-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="5ca65-116">Valige **Salvesta**.</span><span class="sxs-lookup"><span data-stu-id="5ca65-116">Select **Save**.</span></span>
