---
title: Üksuste kopeerimine või ümberpaigutamine SharePointi dokumenditeegis
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807115"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="c0f27-102">Üksuste kopeerimine või ümberpaigutamine SharePointi dokumenditeegis</span><span class="sxs-lookup"><span data-stu-id="c0f27-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="c0f27-103">Dokumenditeegi eri asukohtadesse saate faile, kaustu ja linke kopeerida ja üle viia.</span><span class="sxs-lookup"><span data-stu-id="c0f27-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="c0f27-104">Üksusi saate kopeerida ka üle saitide.</span><span class="sxs-lookup"><span data-stu-id="c0f27-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="c0f27-105">Sirvige brauseris failide, kaustade või linkideni, mida soovite muuta, ja seejärel klõpsake käsku **Kopeeri** või **liigu asukohta**.</span><span class="sxs-lookup"><span data-stu-id="c0f27-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c0f27-106">Kui kasutate SharePoint Online ' i klassikalisi kogemusi, siis **kopeerige** ja **liikuge** pole saadaval.</span><span class="sxs-lookup"><span data-stu-id="c0f27-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="c0f27-107">Valige jaotises **valige sihtkoht**asukoht, kuhu soovite üksused kopeerida või teisaldada või klõpsake saitide täieliku loendi kuvamiseks nuppu **Sirvi saite** .</span><span class="sxs-lookup"><span data-stu-id="c0f27-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c0f27-108">Kui te ei näe üksuste kopeerimisel muid saite, pole saitide kopeerimine konfigureeritud.</span><span class="sxs-lookup"><span data-stu-id="c0f27-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="c0f27-109">Selle lubamiseks avage SharePointi administreerimiskeskuse leht sätted ja klõpsake nuppu **OK**.</span><span class="sxs-lookup"><span data-stu-id="c0f27-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="c0f27-110">Uue kausta loomiseks valige asukoht kausta hierarhias, klõpsake käsku **Uus kaust**, sisestage kausta nimi ja klõpsake nime salvestamiseks märget.</span><span class="sxs-lookup"><span data-stu-id="c0f27-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="c0f27-111">Klõpsake nuppu **Kopeeri siia** või **liikuge siia**.</span><span class="sxs-lookup"><span data-stu-id="c0f27-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c0f27-112">Korraga saate kopeerida kuni 500 MB faile ja kaustu.</span><span class="sxs-lookup"><span data-stu-id="c0f27-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="c0f27-113">>, kui kopeerite dokumente, mis sisaldavad versiooniajalugu, kopeeritakse ainult uusim versioon.</span><span class="sxs-lookup"><span data-stu-id="c0f27-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="c0f27-114">Dokumentide teisaldamisel teisaldatakse ka nende ajalugu.</span><span class="sxs-lookup"><span data-stu-id="c0f27-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="c0f27-115">Kui fail on teisaldatud, kuvatakse see endiselt allika kataloogis, kuni selle sihtkohani teisaldatakse, ja siis see kustutatakse.</span><span class="sxs-lookup"><span data-stu-id="c0f27-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="c0f27-116">Pärast teisaldamist jääb fail pärast teisaldamist prügikasti ja selle suhtes kehtib tavaline Recycle Schedule, kui kasutaja seda prügikastist ei Taasta.</span><span class="sxs-lookup"><span data-stu-id="c0f27-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="c0f27-117">Lisateavet leiate järgmisest teemast.</span><span class="sxs-lookup"><span data-stu-id="c0f27-117">For more information, see:</span></span>

 - <span data-ttu-id="c0f27-118">[Failide paigutamine või kopeerimine SharePointis](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office ' i tugiteenuste artikkel)</span><span class="sxs-lookup"><span data-stu-id="c0f27-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="c0f27-119">[Failide ühest kaustast teise paigutamine](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community Blog artikkel)</span><span class="sxs-lookup"><span data-stu-id="c0f27-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  