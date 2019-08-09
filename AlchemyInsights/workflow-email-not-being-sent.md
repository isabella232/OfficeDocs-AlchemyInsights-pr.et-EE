---
title: Töövoo e-posti ei ole saadetud
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270668"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="ae958-102">Töövoo e-posti ei ole saadetud</span><span class="sxs-lookup"><span data-stu-id="ae958-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="ae958-103">Töövoogude meilisõnumeid ei saadeta kõik kasutajad või ainult teatud kasutajatele või näete viga **e-kirja ei saa saata. Veenduge, et meilisõnumil sobiv adressaat**.</span><span class="sxs-lookup"><span data-stu-id="ae958-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="ae958-104">Kontrollige, kas kasutajal on olemas **Kõigi inimeste** õiguste rühma (kasutaja info loendi) selle saidikogumi.</span><span class="sxs-lookup"><span data-stu-id="ae958-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="ae958-105">Proovi otse URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="ae958-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="ae958-106">Kui kasutaja olemas, veenduge, et kasutaja on sisse logitud lehe.</span><span class="sxs-lookup"><span data-stu-id="ae958-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="ae958-107">Kui on välise kasutaja, veenduge, et nende kutse on aktsepteeritud.</span><span class="sxs-lookup"><span data-stu-id="ae958-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="ae958-108">Kui kasutaja õiguste rühma, veenduge, et meiliaadress on õige.</span><span class="sxs-lookup"><span data-stu-id="ae958-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="ae958-109">Kui kasutajate e-posti aadress ei ole siin seatud, looge selle kasutaja, mis sunnib selle kasutaja konto sünkroonimine SharePointi kasutaja profiilid selles saidikogumis näidisteate.</span><span class="sxs-lookup"><span data-stu-id="ae958-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="ae958-110">Töövoogude meilisõnumeid saadetakse saidi administraatorid, kuid mitte teistele kasutajatele ja kuvada tõrge \*\*Forbidden HTTP- <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="ae958-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="ae958-111">Vaata [Juurdepääs keelatud, kui saadetud e-pakuvad](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="ae958-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="ae958-112">Samuti veenduge, et **piiratud juurdepääsuga kasutaja luba lockdown režiim** saidi kogumise funktsioon pole aktiivne.</span><span class="sxs-lookup"><span data-stu-id="ae958-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="ae958-113">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="ae958-113">Related topics</span></span>
<span data-ttu-id="ae958-114">Tahan proovida Microsoft Flow SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ae958-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ae958-115">Luua voolu</span><span class="sxs-lookup"><span data-stu-id="ae958-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ae958-116">SharePoint ja voolu</span><span class="sxs-lookup"><span data-stu-id="ae958-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


