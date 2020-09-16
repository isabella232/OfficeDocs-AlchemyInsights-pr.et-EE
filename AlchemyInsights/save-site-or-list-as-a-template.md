---
title: Saidi või loendi salvestamine mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: et-EE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727527"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="5cb93-102">Saidi või loendi salvestamine mallina</span><span class="sxs-lookup"><span data-stu-id="5cb93-102">Save site or list as a template</span></span>

<span data-ttu-id="5cb93-103">SharePointi saidi Mallid on eelehitatud määratlused, mis on mõeldud teatud ärivajaduse ümber.</span><span class="sxs-lookup"><span data-stu-id="5cb93-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="5cb93-104">Lisateavet leiate teemast [mallide kasutamine eri tüüpi SharePointi saitide loomiseks](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="5cb93-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="5cb93-105">Siin on mõned levinud probleemid/lahendused seoses saidi või loendi salvestamisega mallina SharePoint Online ' is.</span><span class="sxs-lookup"><span data-stu-id="5cb93-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="5cb93-106">**Nupp Salvesta saidi/loendi Mall pole saadaval või puudub**.</span><span class="sxs-lookup"><span data-stu-id="5cb93-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="5cb93-107">Administraatorid peavad lubama kohandatud skripti malli funktsioonide lubamiseks.</span><span class="sxs-lookup"><span data-stu-id="5cb93-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="5cb93-108">Üksikasjalikud juhised leiate teemast [kohandatud skripti lubamine või keelamine](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="5cb93-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="5cb93-109">Käsk Salvesta sait mallina pole toetatud ja võib põhjustada probleeme saitidel, mis kasutavad SharePoint Serveri avaldamise infrastruktuuri.</span><span class="sxs-lookup"><span data-stu-id="5cb93-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="5cb93-110">**Saidimalli ei saa luua või see ei tööta õigesti**</span><span class="sxs-lookup"><span data-stu-id="5cb93-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="5cb93-111">Mallil võib olla [funktsioon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) puudu ja see ei aktiveeru.</span><span class="sxs-lookup"><span data-stu-id="5cb93-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="5cb93-112">Kui funktsioon pole praeguses saidikogumis aktiveerimiseks saadaval, ei saa te saiti saidi loomiseks kasutada.</span><span class="sxs-lookup"><span data-stu-id="5cb93-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="5cb93-113">Saate vaadata, kas loendid või teegid ületavad 5000 üksuste [loendivaate](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) piirmäära, kuna see võib saidi malli loomist blokeerida.</span><span class="sxs-lookup"><span data-stu-id="5cb93-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="5cb93-114">Sait võib kasutada liiga palju ressursse ja seetõttu on saidimall üle 50 megabaidi (MB) limiidi.</span><span class="sxs-lookup"><span data-stu-id="5cb93-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="5cb93-115">On probleeme, mis kuvavad andmeid otsinguveeru kasutavast loendist.</span><span class="sxs-lookup"><span data-stu-id="5cb93-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="5cb93-116">Lisateavet leiate teemast [mallide põhjal loodud loend ei kuva SharePoint Online ' is õigete otsinguväljade andmeid](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="5cb93-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="5cb93-117">Üksikasjalikumat teavet levinud probleemide ja lahenduste kohta leiate teemast [saidimallide loomine ja kasutamine](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="5cb93-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

