---
title: Töövoo e-posti ei saadeta
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049369"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="98c5e-102">Töövoo e-posti ei saadeta SharePointi loendi või teegi</span><span class="sxs-lookup"><span data-stu-id="98c5e-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="98c5e-103">Töövoogude e-posti ei saadeta kõigile kasutajatele või ainult teatud kasutajatele või kuvatakse tõrge **meilisõnumit ei saa saata. Veenduge, et meilisõnumil oleks kehtiv adressaat**.</span><span class="sxs-lookup"><span data-stu-id="98c5e-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="98c5e-104">Kontrollige, kas kasutaja on olemas selle saidikogumi **kõik inimesed** õigused rühma (kasutaja teabe loend).</span><span class="sxs-lookup"><span data-stu-id="98c5e-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="98c5e-105">Näidis Direct URL: https://<tenant>. sharepoint.com/sites/<sitename>/_Layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="98c5e-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="98c5e-106">Kui kasutajat pole olemas, veenduge, et kasutaja on lehele sisse logitud.</span><span class="sxs-lookup"><span data-stu-id="98c5e-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="98c5e-107">Kui see on väline kasutaja, veenduge, et nende kutse on aktsepteeritud.</span><span class="sxs-lookup"><span data-stu-id="98c5e-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="98c5e-108">Kui kasutaja on olemas õiguste rühma, veenduge, et e-posti aadress on õige.</span><span class="sxs-lookup"><span data-stu-id="98c5e-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="98c5e-109">Kui kasutaja e-posti aadress on seatud siin, siis luua selle kasutaja näidisteatis, mis sunnib selle kasutajakonto sünkroonimine SharePointi kasutajaprofiilid selle saidikogumi.</span><span class="sxs-lookup"><span data-stu-id="98c5e-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="98c5e-110">E-posti töövoogude saadetakse saidikogumi administraatorid, kuid mitte teiste kasutajate ja **http keelatud <span>https</span>-i tõrge://URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendEmail**.</span><span class="sxs-lookup"><span data-stu-id="98c5e-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="98c5e-111">Vaadake [juurdepääs keelatud, kui saadate e-kirja SharePointi rühma](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="98c5e-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="98c5e-112">Samuti veenduge, et **piiratud juurdepääsuga kasutaja õiguste Lockdown režiimi** saidikogumi funktsioon ei ole aktiivne.</span><span class="sxs-lookup"><span data-stu-id="98c5e-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="98c5e-113">Seotud teemad</span><span class="sxs-lookup"><span data-stu-id="98c5e-113">Related topics</span></span>
<span data-ttu-id="98c5e-114">Soovite proovida Microsoft Flow SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="98c5e-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="98c5e-115">Voo loomine</span><span class="sxs-lookup"><span data-stu-id="98c5e-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="98c5e-116">SharePointi ja voog</span><span class="sxs-lookup"><span data-stu-id="98c5e-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


