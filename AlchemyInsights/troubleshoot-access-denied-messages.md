---
title: Accessi keelatud sõnumite tõrkeotsing
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690779"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="c366e-102">Accessi keelatud sõnumite tõrkeotsing</span><span class="sxs-lookup"><span data-stu-id="c366e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="c366e-103">Kui keegi sai SharePointi ühiskausta teate "juurdepääs keelatud", võib saidikogumi administraator lubada "piiratud juurdepääsuga kasutaja õiguste lukustamise režiimi".</span><span class="sxs-lookup"><span data-stu-id="c366e-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="c366e-104">Selle väljalülitamiseks tehke järgmist.</span><span class="sxs-lookup"><span data-stu-id="c366e-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="c366e-105">Sirvige saidini, klõpsake ikooni sätted ja seejärel käsku **saidi sätted**.</span><span class="sxs-lookup"><span data-stu-id="c366e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="c366e-106">Klõpsake jaotises **Saidikogumi administreerimine**linki **saidikogumi funktsioonid**.</span><span class="sxs-lookup"><span data-stu-id="c366e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="c366e-107">Klõpsake **piiratud juurdepääsuga kasutaja õiguste lukustamise režiimi**kõrval nuppu **Desaktiveeri**.</span><span class="sxs-lookup"><span data-stu-id="c366e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="c366e-108">Kui sait on avaldamise sait, võib ka ühiskaustade korral tekkida juurdepääs keelatud.</span><span class="sxs-lookup"><span data-stu-id="c366e-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="c366e-109">Lisateavet leiate teemast [juurdepääs keelatud ühiskausta](https://go.microsoft.com/fwlink/?linkid=2004317)avamisel.</span><span class="sxs-lookup"><span data-stu-id="c366e-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="c366e-110">Kui keegi sai Accessi päringute vaatamise katsel sõnumi "juurdepääs keelatud", tuleb kasutaja lisada saidi saidikogumi administraatoriks või rühma omanike liikmeks.</span><span class="sxs-lookup"><span data-stu-id="c366e-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="c366e-111">Lisateavet leiate teemast Accessi [taotluste loendisse juurdepääs keelatud](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="c366e-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="c366e-112">Kui kasutaja sai tõrketeate "juurdepääs keelatud" pärast seda, kui need on kohapealt Active Directoryst eemaldatud ja seejärel tagasi lisatud, lugege teemat [juurdepääs on keelatud, kui kasutajakonto sünkroonitakse Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="c366e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

