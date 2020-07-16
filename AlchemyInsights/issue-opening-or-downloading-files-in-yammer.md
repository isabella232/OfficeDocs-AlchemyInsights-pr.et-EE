---
title: Probleem failide avamisel või allalaadimisel Yammeris
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148248"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="d3afc-102">Probleem failide avamisel või allalaadimisel Yammeris</span><span class="sxs-lookup"><span data-stu-id="d3afc-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="d3afc-103">Klassikaline Yammer toetab sõnumitesse ja rühmadesse failide üleslaadimise mitut suvandit.</span><span class="sxs-lookup"><span data-stu-id="d3afc-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="d3afc-104">Sõltuvalt võrgu konfiguratsioonist on failide vaikemälu SharePointis.</span><span class="sxs-lookup"><span data-stu-id="d3afc-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="d3afc-105">Uue Yammeri failivalija ei toeta veel kõiki klassikalises Yammeris saadaolevaid suvandeid.</span><span class="sxs-lookup"><span data-stu-id="d3afc-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="d3afc-106">Tulevane värskendus lisab täiendavaid funktsioone.</span><span class="sxs-lookup"><span data-stu-id="d3afc-106">A future update will add additional features.</span></span> <span data-ttu-id="d3afc-107">Lisateavet leiate teemast [Faili või pildi manustamine Yammeri vestluse postitusse](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="d3afc-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="d3afc-108">**Faili ei saa avada ega alla laadida**</span><span class="sxs-lookup"><span data-stu-id="d3afc-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="d3afc-109">Fail võib yammerisse üles laadida, kuid linkida ka SharePoint Online'i failiga.</span><span class="sxs-lookup"><span data-stu-id="d3afc-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="d3afc-110">Tõrkeotsingu sooritamiseks peate esmalt määrama faili asukoha.</span><span class="sxs-lookup"><span data-stu-id="d3afc-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="d3afc-111">Kui fail on Yammerisse üles laaditud, on sellel URL \*.yammer.com.</span><span class="sxs-lookup"><span data-stu-id="d3afc-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="d3afc-112">Veenduge, et nõutavad URL-id ja IP-aadressid on blokeeritud.</span><span class="sxs-lookup"><span data-stu-id="d3afc-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="d3afc-113">Lisateavet leiate ajaveebipostitusest [Yammeri püsiprogrammeeritud IP-aadresside kasutamine pole soovitatav.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)</span><span class="sxs-lookup"><span data-stu-id="d3afc-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="d3afc-114">Kontrollige, kas faili saab alla laadida ka üldadministraator.</span><span class="sxs-lookup"><span data-stu-id="d3afc-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="d3afc-115">Kui fail on privaatne, peate võib-olla kasutama privaatse sisu režiimi.</span><span class="sxs-lookup"><span data-stu-id="d3afc-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="d3afc-116">Lisateavet leiate teemast [Yammeri privaatse sisu jälgimine](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="d3afc-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="d3afc-117">**Yammeri võrgutasandi külalised ja failid SharePoint Online'is**</span><span class="sxs-lookup"><span data-stu-id="d3afc-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="d3afc-118">[Yammeri võrgutasandi külalised](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ei kasuta Azure AD B2B ja on Yammeri teenuse sisemine, et nad ei pääse Yammeri failidele, mis on talletatud SharePointis.</span><span class="sxs-lookup"><span data-stu-id="d3afc-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="d3afc-119">Looge väline AAD B2B kasutaja, kellel on juurdepääs dokumenditeekidele SharePoint Online'is, kasutades seda identiteeti.</span><span class="sxs-lookup"><span data-stu-id="d3afc-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="d3afc-120">Lisateavet Yammeri tulevase Azure AD B2B külalistoe kohta leiate teemast [Ettevõttest ettevõtteni (B2B) külaline yammeri eelvaates – klienditingimused ja KKK](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="d3afc-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>