---
title: SharePoint Online ' i ahendamine
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773843"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="8097e-102">SharePoint Online ' i ahendamine</span><span class="sxs-lookup"><span data-stu-id="8097e-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="8097e-103">**Tähtis**! Nende enneolematude aegade jooksul võtame kasutusele meetmed, et säilitada SharePoint Online’i ja OneDrive’i teenuste hea kättesadavus. Lisateabe saamiseks vaadake teemat [SharePoint Online’i ajutised funktsioonide muudatused](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="8097e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8097e-104">**503 server on hõivatud tõrge**</span><span class="sxs-lookup"><span data-stu-id="8097e-104">**503 server is busy error**</span></span>

<span data-ttu-id="8097e-105">Kui proovite liikuda SharePointi või OneDrive ' i saitidele, võivad kasutajad saada 503 serveriga hõivatud tõrke.</span><span class="sxs-lookup"><span data-stu-id="8097e-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="8097e-106">Selle tõrke põhjuseks võib olla SharePointi teenuse ahendamine.</span><span class="sxs-lookup"><span data-stu-id="8097e-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="8097e-107">SharePoint Online kasutab SharePoint Online’i teenuste optimaalse jõudluse ja töökindluse säilitamiseks ahendamist.</span><span class="sxs-lookup"><span data-stu-id="8097e-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="8097e-108">Ahendamine piirab kasutajate toimingute või samaaegsete kõnede arvu (skripti või koodi poolt), et ennetada ressursside ülekasutamist.</span><span class="sxs-lookup"><span data-stu-id="8097e-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="8097e-109">Lisateavet ahendamise kohta leiate artiklist [SharePoint Online ' is ahendamise või blokeerimise vältimine](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="8097e-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="8097e-110">Kui arvate [, et see](https://portal.office.com/adminportal/home#/MessageCenter)tõrge pole seotud ahendamisega, saate kontrollida, kas teie Rentnik on teie rentniku jaoks aktiivset hooldust otsinud.</span><span class="sxs-lookup"><span data-stu-id="8097e-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="8097e-111">Lõpetuseks veenduge, et külastate [teenuse Health](https://portal.office.com/adminportal/home#/servicehealth) lehte, et kontrollida mis tahes nõuandjaid/juhtumeid, mis võivad toimuda.</span><span class="sxs-lookup"><span data-stu-id="8097e-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

