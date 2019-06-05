---
title: Kuidas TenantAccessBlockedException viga, kui e-posti juurdepääsu 127?
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 54ebc269b391e6b0d607e55af8283ebf3d9e2aa7
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715068"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="63af0-102">Hooldus sõnumi kui üritatakse kasutada OneDrive'i või SharePointi kirjutuskaitstud</span><span class="sxs-lookup"><span data-stu-id="63af0-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="63af0-103">Kasutajatele võidakse kuvada Read-Only hooldus sõnumi, kui üritatakse kasutada OneDrive'i või SharePointi.</span><span class="sxs-lookup"><span data-stu-id="63af0-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="63af0-104">Kontrollida, kas aktiivne hooldus toimub teie rentniku <a href="https://portal.office.com/adminportal/home#/MessageCenter">sõnumikeskuse</a>kaudu.</span><span class="sxs-lookup"><span data-stu-id="63af0-104">Check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>.</span></span> <span data-ttu-id="63af0-105">Lõpuks tagama kontrollimiseks mis tahes teateid/intsidente, mis võib aset <a href="https://portal.office.com/adminportal/home#/servicehealth">Teenuseid tervise</a> lehte külastades.</span><span class="sxs-lookup"><span data-stu-id="63af0-105">Finally, ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="63af0-106">Kui keskus ja teenuste seisundi armatuurlaud ei täheldanud midagi jooksvaks hoolduseks oma üürnikule, võib see olla brauseri caching küsimus.</span><span class="sxs-lookup"><span data-stu-id="63af0-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="63af0-107">Proovige enne saidil navigeerimise brauseri vahemälu tühjendamine.</span><span class="sxs-lookup"><span data-stu-id="63af0-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

  <li><span data-ttu-id="63af0-108">Microsoft Edge brauser, külastage <strong>rohkem &hellip; &gt; sätted</strong></span><span class="sxs-lookup"><span data-stu-id="63af0-108">In the Microsoft Edge browser, go to <strong>More &hellip;&gt; Settings</strong></span></span></li>  <li><span data-ttu-id="63af0-109">Valige jaotises <strong>selge sirvimiseks </strong> <strong>Valige kustutatav</strong>.</span><span class="sxs-lookup"><span data-stu-id="63af0-109">Under <strong>Clear browsing </strong>, select <strong>Choose what to clear</strong>.</span></span></li>  <li><span data-ttu-id="63af0-110">Valige küpsised ja salvestatud veebisaidiandmed ja valige <strong>selge</strong>.</span><span class="sxs-lookup"><span data-stu-id="63af0-110">Select the Cookies and saved website data check box and select <strong>Clear</strong>.</span></span></li>  </ol>  

<span data-ttu-id="63af0-111">**Märkus**: järgmiselt võivad erineda kasutades teisi brauserid nagu Firefox või Chrome.</span><span class="sxs-lookup"><span data-stu-id="63af0-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

