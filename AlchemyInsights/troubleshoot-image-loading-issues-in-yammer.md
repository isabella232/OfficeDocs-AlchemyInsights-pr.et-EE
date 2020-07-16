---
title: Piltide laadimise probleemide tõrkeotsing Yammeris
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148226"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="d038f-102">Piltide laadimise probleemide tõrkeotsing Yammeris</span><span class="sxs-lookup"><span data-stu-id="d038f-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="d038f-103">Kui yammeris fotode ja faili eelvaadetega probleemid ilmnevad, tehke tõrkeotsingut, kontrollides, kas probleem ilmneb kõigi kasutajate puhul, kas see esineb mobiilseadmetes ja kas see on manuse üleslaadimisel reprodutseeritav.</span><span class="sxs-lookup"><span data-stu-id="d038f-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="d038f-104">**Profiili fotoprobleemid**</span><span class="sxs-lookup"><span data-stu-id="d038f-104">**Profile photo issues**</span></span>  

<span data-ttu-id="d038f-105">Kui lõppkasutajad logivad Yammerisse sisse Microsoft 365 kaudu, peavad nad muutma oma profiili, sealhulgas oma profiilifotot.</span><span class="sxs-lookup"><span data-stu-id="d038f-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="d038f-106">Kui kasutajatel pole lubatud profiilivärskendusi teha, saab administraator teha kasutaja jaoks värskenduse.</span><span class="sxs-lookup"><span data-stu-id="d038f-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="d038f-107">Lisateavet leiate teemast [Profiili vaatamine ja värskendamine Office Delve'is](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="d038f-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="d038f-108">Lisateavet profiilide redigeerimise (sh profiilifotode) kohta leiate teemast [Yammeri profiili ja sätete muutmine](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="d038f-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="d038f-109">Värskendatud profiilifotod sünkroonitakse profiiliatribuutidest erinevalt.</span><span class="sxs-lookup"><span data-stu-id="d038f-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="d038f-110">Kasutajad peavad oma profiilifoto sünkroonimise algatamiseks sisse logima.</span><span class="sxs-lookup"><span data-stu-id="d038f-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="d038f-111">Lisateavet leiate teemast [Kasutajaprofiili pildid värskendatakse teenusekomplektist Office 365 Yammerisse.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)</span><span class="sxs-lookup"><span data-stu-id="d038f-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="d038f-112">Lisateavet Yammeri kasutaja elutsükli kohta leiate teemast [Yammeri kasutajate haldamine kogu nende elutsükli jooksul teenusekomplektist Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="d038f-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="d038f-113">Lisateavet profiilipildi sünkroonimise microsoft 365-s toimimise kohta leiate teemast [Teave profiilipildi sünkroonimise kohta rakenduses Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="d038f-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="d038f-114">**Dokumendi eelvaated ja pildi pisipildi probleemid**</span><span class="sxs-lookup"><span data-stu-id="d038f-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="d038f-115">Kui failid või pildid on Yammerisse postitatud, ei pruugita eelvaateid kuvada, kuna:</span><span class="sxs-lookup"><span data-stu-id="d038f-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="d038f-116">Fail on rikutud ja seda ei saa töödelda.</span><span class="sxs-lookup"><span data-stu-id="d038f-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="d038f-117">Faili pole hiljuti SharePoint Online'i üles laaditud või Yammeril on muudel põhjustel sobimatud metaandmed.</span><span class="sxs-lookup"><span data-stu-id="d038f-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="d038f-118">eelvaatepiltide laadimiseks vajalikud URL-id on blokeeritud.</span><span class="sxs-lookup"><span data-stu-id="d038f-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="d038f-119">Kasutaja eemaldas faili eelvaate enne sisestamist.</span><span class="sxs-lookup"><span data-stu-id="d038f-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="d038f-120">Teenuseprobleem takistas eelvaate loomist.</span><span class="sxs-lookup"><span data-stu-id="d038f-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="d038f-121">**Märkus** Linkide ja failide üleslaadimiste eelvaated võivad käituda erinevalt.</span><span class="sxs-lookup"><span data-stu-id="d038f-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="d038f-122">Linke internetis olevatele failidele või täiendavaid autentimist nõudvaid linke ei pruugita õigesti kuvada.</span><span class="sxs-lookup"><span data-stu-id="d038f-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="d038f-123">Lisateavet leiate teemast [Faili või pildi manustamine Yammeri sõnumile](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="d038f-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 