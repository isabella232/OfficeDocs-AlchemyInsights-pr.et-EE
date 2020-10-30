---
title: Tellimuse juurdepääs
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807293"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="0ddc6-102">Azure ' i probleemide tõttu ei saa Azure ' i sisse logida (brauser hangub, keerutab, ei laadi jne).</span><span class="sxs-lookup"><span data-stu-id="0ddc6-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="0ddc6-103">Võib juhtuda, et seisak mõjutab katkestust.</span><span class="sxs-lookup"><span data-stu-id="0ddc6-103">You might be impacted by an outage.</span></span> <span data-ttu-id="0ddc6-104">Palun kontrolli, kas käimas on katkestus: [Azure ' i tervislik seisund](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="0ddc6-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="0ddc6-105">Logige kõik aktiivsed Azure ' i seansid välja.</span><span class="sxs-lookup"><span data-stu-id="0ddc6-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="0ddc6-106">Alustage oma veebibrauseri privaatset või inkognito režiimi.</span><span class="sxs-lookup"><span data-stu-id="0ddc6-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="0ddc6-107">Samuti võite proovida värskendada brauserit, kasutada mõnda muud brauserit, kustutada vahemälu küpsised, kui need ei tööta.</span><span class="sxs-lookup"><span data-stu-id="0ddc6-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="0ddc6-108">Lisateave: [Sisselogimistega seotud probleemide tõrkeotsing](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="0ddc6-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="0ddc6-109">**Tellimusele ei pääse juurde**</span><span class="sxs-lookup"><span data-stu-id="0ddc6-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="0ddc6-110">Veenduge, et [Azure ' i portaalis](https://portal.azure.com/)oleks valitud õige Azure ' i kataloog paremas ülanurgas olevast kontost.</span><span class="sxs-lookup"><span data-stu-id="0ddc6-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="0ddc6-111">Veenduge, et [Azure ' i konto keskuses](https://account.windowsazure.com/Subscriptions)oleks konto administraator.</span><span class="sxs-lookup"><span data-stu-id="0ddc6-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="0ddc6-112">Lisateave: [leitud tellimuste tõrkeotsing](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="0ddc6-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="0ddc6-113">**Arvelduste ajaloole ei saa juurde pääseda**</span><span class="sxs-lookup"><span data-stu-id="0ddc6-113">**Unable to access billing history**</span></span>

<span data-ttu-id="0ddc6-114">Konto administraator peab veenduma, et arvelduse teabe kasutajaks olev kasutaja on lisatud Azure Active Directorysse külalisena kasutajana: [uue kasutaja lisamine või kustutamine](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0ddc6-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0ddc6-115">Seejärel peab kasutajale andma üldise administraatori rolli: [määrata kasutajatele rolli](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0ddc6-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0ddc6-116">Postitage see, kasutaja saab anda arvelduse juurdepääsu RBAC poliitika kaudu: [anda juurdepääsu Arveldusele](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="0ddc6-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="0ddc6-117">**Soovitatavad dokumendid**</span><span class="sxs-lookup"><span data-stu-id="0ddc6-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="0ddc6-118">Ma ei saa oma Azure ' i tellimuse haldamiseks sisse logida</span><span class="sxs-lookup"><span data-stu-id="0ddc6-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)